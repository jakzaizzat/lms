<template>
    <div>
        <Card header="Add New Account">
            <template slot="content">
                <div class="p-8">

                    <div class="flex mb-6">
                        <div class="w-1/3 flex">
                            <label class="block uppercase tracking-wide text-black text-xs font-bold mb-2" for="grid-first-name">
                            Name
                            </label>
                        </div>
                        <div class="w-2/3">
                            <input type="text" class="appearance-none block w-full bg-grey-lighter text-grey-darker rounded py-3 px-4 mb-3 leading-tight focus:outline-none" />
                        </div>
                    </div>

                    <div class="flex mb-6">
                        <div class="w-1/3 flex">
                            <label class="block uppercase tracking-wide text-black text-xs font-bold mb-2" for="grid-first-name">
                                Department
                            </label>
                        </div>

                        <div class="w-2/3">
                            <select  class="appearance-none block w-full bg-grey-lighter text-grey-darker rounded py-3 px-4 mb-3 leading-tight focus:outline-none" >
                                <option>IT</option>
                                <option>Finance</option>
                                <option>Admin</option>
                            </select>
                        </div>
                    </div>

                    <div class="flex mb-6">
                        <div class="w-1/3 flex">
                            <label class="block uppercase tracking-wide text-black text-xs font-bold mb-2" for="grid-first-name">
                            Position
                            </label>
                        </div>

                        <div class="w-2/3">
                            <input type="text" class="appearance-none block w-full bg-grey-lighter text-grey-darker rounded py-3 px-4 mb-3 leading-tight focus:outline-none" />
                        </div>
                    </div>

                    <div class="flex mb-6">
                        <div class="w-1/3 flex">
                            <label class="block uppercase tracking-wide text-black text-xs font-bold mb-2" for="grid-first-name">
                            Medical Leave
                            </label>
                        </div>

                        <div class="w-2/3">
                            <input type="number" class="appearance-none block w-full bg-grey-lighter text-grey-darker rounded py-3 px-4 mb-3 leading-tight focus:outline-none" />
                        </div>
                    </div>

                    <div class="flex mb-6">
                        <div class="w-1/3 flex">
                            <label class="block uppercase tracking-wide text-black text-xs font-bold mb-2" for="grid-first-name">
                            Annual Leave
                            </label>
                        </div>

                        <div class="w-2/3">
                            <input type="number" class="appearance-none block w-full bg-grey-lighter text-grey-darker rounded py-3 px-4 mb-3 leading-tight focus:outline-none" />
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
