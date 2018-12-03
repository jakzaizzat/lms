<template>
    <div>
        <Card header="Apply Leave">
            <template slot="content">
                <div class="p-8">

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
                            <textarea class="appearance-none block w-full bg-grey-lighter text-grey-darker rounded py-3 px-4 mb-3 leading-tight focus:outline-none" rows="5"></textarea>
                        </div>
                    </div>

                    <div class="flex mb-6">
                        <div class="w-1/3 flex">
                            <label class="block uppercase tracking-wide text-black text-xs font-bold mb-2" for="grid-first-name">
                                Contacts details during leave
                                <p class="normal-case font-normal mt-2 text-grey-dark">If something happens and urgently need your details</p>
                            </label>
                        </div>
                        <div class="w-2/3">
                            <input type="text" class="appearance-none block w-full bg-grey-lighter text-grey-darker rounded py-3 px-4 mb-3 leading-tight focus:outline-none" />
                        </div>
                    </div>

                    <div class="flex mb-6">
                        <div class="w-1/3 flex">
                            <label class="block uppercase tracking-wide text-black text-xs font-bold mb-2" for="grid-first-name">
                                Date
                            </label>
                        </div>
                        <div class="w-2/3">
                            <button class="flex items-center no-underline border-primary text-primary text-center bg-white group font-bold rounded py-2 px-4 nuxt-link-exact-active nuxt-link-active">Select a date</button>
                        </div>
                    </div>

                    <div class="flex mb-6">
                        <div class="w-1/3 flex">
                            <label class="block uppercase tracking-wide text-black text-xs font-bold mb-2" for="grid-first-name">
                            Type of Leave
                            </label>
                        </div>
                        <div class="w-2/3">
                            <div class="mb-5">
                                <input type="checkbox" />
                                <span class="ml-3 bg-green-lighter text-green-darkest font-bold rounded-full text-sm p-1">14</span>
                                <span class="pl-3 text-grey-dark">Annual Leave</span>
                            </div>
                            <div class="mb-5">
                                <input type="checkbox" />
                                <span class="ml-3 bg-red-lighter text-red-darkest font-bold rounded-full text-sm p-1">14</span>
                                <span class="pl-3 text-grey-dark">Medical Leave</span>
                            </div>
                            <div class="mb-5">
                                <input type="checkbox" />
                                <span class="ml-3 bg-grey-lighter text-grey-darkest font-bold rounded-full text-sm p-1">14</span>
                                <span class="pl-3 text-grey-dark">Emergency Leave</span>
                            </div>
                        </div>
                    </div>
                </div>
            </template>


            <template slot="footer">
                <div class="flex justify-end py-4">
                    <a class="flex justify-center items-center no-underline text-white text-center bg-primary group font-bold rounded py-2 nuxt-link-exact-active nuxt-link-active px-4" href="/apply/confirmation">Submit</a>
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
    }
}
</script>
