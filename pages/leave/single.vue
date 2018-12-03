<template>
    <div>
        <Card header="Leave #01">
            <template slot="content">
                <div class="p-8">
                    <div class="bg-orange-lightest border-l-4 border-orange text-orange-dark p-4 mb-8" role="alert">
                        <p>Waiting for <span class="font-bold">HR Manager</span> to approve</p>
                    </div>

                    <div class="flex mb-6">
                        <div class="w-1/3 flex">
                            <label class="block uppercase tracking-wide text-black text-xs font-bold mb-2" for="grid-first-name">
                            Name
                            </label>
                        </div>
                        <div class="w-2/3">
                            <span class="font-bold text-grey-darkest">Mohd Aizzat Bin Mohd Zulkifli</span>
                        </div>
                    </div>

                    <div class="flex mb-6">
                        <div class="w-1/3 flex">
                            <label class="block uppercase tracking-wide text-black text-xs font-bold mb-2" for="grid-first-name">
                                Department
                            </label>
                        </div>
                        <div class="w-2/3">
                            <span class="font-bold text-grey-darkest">IT TECH</span>
                        </div>
                    </div>

                    <div class="flex mb-6">
                        <div class="w-1/3 flex">
                            <label class="block uppercase tracking-wide text-black text-xs font-bold mb-2" for="grid-first-name">
                            Position
                            </label>
                        </div>
                        <div class="w-2/3">
                            <span class="font-bold text-grey-darkest">Software Developer</span>
                        </div>
                    </div>

                    <div class="flex mb-6">
                        <div class="w-1/3 flex">
                            <label class="block uppercase tracking-wide text-black text-xs font-bold mb-2" for="grid-first-name">
                            Reason (s)
                            </label>
                        </div>
                        <div class="w-2/3">
                            <span class="font-bold text-grey-darkest">Balik Terengganu</span>
                        </div>
                    </div>

                    <div class="flex mb-6">
                        <div class="w-1/3 flex">
                            <label class="block uppercase tracking-wide text-black text-xs font-bold mb-2" for="grid-first-name">
                                Contacts details during leave
                            </label>
                        </div>
                        <div class="w-2/3">
                            <span class="font-bold text-grey-darkest">0145142241</span>
                        </div>
                    </div>

                    <div class="flex mb-6">
                        <div class="w-1/3 flex">
                            <label class="block uppercase tracking-wide text-black text-xs font-bold mb-2" for="grid-first-name">
                                Date
                            </label>
                        </div>
                        <div class="w-2/3">
                            <span class="font-bold text-grey-darkest">06 December 2018 untill 12 December 2018</span>
                        </div>
                    </div>

                    <div class="flex mb-6">
                        <div class="w-1/3 flex">
                            <label class="block uppercase tracking-wide text-black text-xs font-bold mb-2" for="grid-first-name">
                                Approval
                            </label>
                        </div>
                        <div class="w-2/3">
                            <div class="flex items-center mb-2">
                                <svg class="fill-current text-green-dark" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24"><path class="heroicon-ui" d="M12 22a10 10 0 1 1 0-20 10 10 0 0 1 0 20zm0-2a8 8 0 1 0 0-16 8 8 0 0 0 0 16zm-2.3-8.7l1.3 1.29 3.3-3.3a1 1 0 0 1 1.4 1.42l-4 4a1 1 0 0 1-1.4 0l-2-2a1 1 0 0 1 1.4-1.42z"/></svg>
                                <span class="font-bold text-grey-darkest pl-3">Umar Mukhtar</span>
                            </div>
                            <div class="flex items-center mb-2">
                                <svg class="fill-current text-grey" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24"><path class="heroicon-ui" d="M12 22a10 10 0 1 1 0-20 10 10 0 0 1 0 20zm0-2a8 8 0 1 0 0-16 8 8 0 0 0 0 16zm-2.3-8.7l1.3 1.29 3.3-3.3a1 1 0 0 1 1.4 1.42l-4 4a1 1 0 0 1-1.4 0l-2-2a1 1 0 0 1 1.4-1.42z"/></svg>
                                <span class="font-bold text-grey pl-3">HR Manager</span>
                            </div>
                        </div>
                    </div>
                </div>
            </template>
        </Card>
    </div>
</template>

<script>
import Card from '~/components/Card.vue'
export default {
    layout: 'dashboard',
    components: {
        Card
    },
    methods: {
      undo() {
        this.$refs.signaturePad.undoSignature();
      },
      save() {
        const { isEmpty, data } = this.$refs.signaturePad.saveSignature();
        console.log(isEmpty);
        console.log(data);
      }
    }
}
</script>

<style>
#signature {
  border: double 3px transparent;
  border-radius: 5px;
  background-image: linear-gradient(white, white),
    radial-gradient(circle at top left, #4bc5e8, #9f6274);
  background-origin: border-box;
  background-clip: content-box, border-box;
}
</style>
