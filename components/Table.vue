<template>
    <div class="table w-full">
        <div class="table--header flex px-8 py-2 text-left text-xs font-bold tracking-wide text-grey-darkest uppercase">
            <div class="flex-1 items-center">
                <span>Name</span>
            </div>
            <div class="flex-1 px-4 items-center">
                <span>From</span>
            </div>
            <div class="flex-1 px-4 items-center">
                <span>To</span>
            </div>
            <div class="flex px-4 items-center">
                <span>Status</span>
            </div>
        </div>
        <div
            v-for="app in applications" v-bind:key="app.id"
            class="table--content flex px-8 py-2 text-xs text-grey-darkest text-sm">
            <div class="flex-1 items-center">
                <div class="flex items-center py-2">
                    <img src="https://pingping.io/storage/favicons/9OjmlyedrWinH18b.png"/>
                    <div class="pl-2 leading-normal">
                        <div class="font-bold text-black">{{ app.name }}</div>
                        <div class="">{{ app.department }}</div>
                    </div>
                </div>
            </div>
            <div class="flex flex-1 py-2 px-4 items-center">
                <span>{{ app.from }}</span>
            </div>
            <div class="flex flex-1 py-2 px-4 items-center">
                <span>{{ app.to }}</span>
            </div>
            <div class="flex px-4 items-center justify-center">
                <a href="#" class="text-primary font-bold no-underline">Manage</a>
            </div>
        </div>
    </div>
</template>


<style>
    .table--header{
        background-color: #f0f4f9;
    }
</style>


<script>
export default {
    data() {
        return {
            applications: [
                {
                    id: 1,
                    name: "Mohd Aizzat Mohd Zulkifli",
                    department: "IT Dept",
                    from: "6 December 2018",
                    to: "16 December 2018"
                },
                {
                    id: 2,
                    name: "Mohd Aidil Zulkifli",
                    department: "IT Dept",
                    from: "6 December 2018",
                    to: "16 December 2018"
                },
                {
                    id: 3,
                    name: "Atiq Mohd Zulkifli",
                    department: "IT Dept",
                    from: "6 December 2018",
                    to: "16 December 2018"
                }
            ]
        }
    }
}
</script>
