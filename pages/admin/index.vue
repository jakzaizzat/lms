<template>
  <div class="container mx-auto px-6">

        <Card header="Needs Approval">
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
