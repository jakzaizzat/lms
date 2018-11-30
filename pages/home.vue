<template>
  <div class="container mx-auto px-6">
        <div class="flex -mx-4 mb-8">
            <div class="flex flex-col card flex-1 text-center py-6 mx-4">
                <div class="text-grey-dark text-sm uppercase text-center font-bold tracking-wider mb-2 md:text-md">Leave Usage</div>
                <span class="flex flex-1 py-2 px-4 font-bold rounded text-center text-lg uppercase items-center justify-center mx-6 my-2 bg-green-lighter text-green-darker">3</span>
            </div>
            <div class="flex flex-col card flex-1 text-center py-6 mx-4">
                <div class="text-grey-dark text-sm uppercase text-center font-bold tracking-wider mb-2 md:text-md">Emergency Leave</div>
                <span class="flex flex-1 py-2 px-4 font-bold rounded text-center text-lg uppercase items-center justify-center mx-6 my-2 bg-grey-lighter text-grey-darker">0</span>
            </div>
            <div class="flex flex-col card flex-1 text-center py-6 mx-4">
                <div class="text-grey-dark text-sm uppercase text-center font-bold tracking-wider mb-2 md:text-md">Annual Leave</div>
                <span class="flex flex-1 py-2 px-4 font-bold rounded text-center text-lg uppercase items-center justify-center mx-6 my-2 bg-green-lighter text-green-darker">3</span>
            </div>
        </div>

        <Card header="History Application">
            <template slot="content">
                <Table/>
            </template>

            <template slot="footer">
                <div class="flex justify-between py-8">
                    <a class="font-medium text-primary hover:text-primary-dark no-underline" href="#">Don't have account yet</a>
                    <a class="text-grey-darkest hover:text-black no-underline" href="#">Forgot Password</a>
                </div>
            </template>
        </Card>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Nav from '~/components/Nav.vue'
import Card from '~/components/Card.vue'
import Table from '~/components/Table.vue'

export default {
    layout: 'dashboard',
    components: {
        Logo,
        Nav,
        Card,
        Table
    }
}
</script>
