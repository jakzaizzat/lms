<template>
  <div class="container mx-auto px-6">

        <Card header="Recent Applications">
            <template slot="content">
                <Table/>
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
