<template>
  <div class="container mx-auto px-6">
        <div class="flex -mx-4 mb-8">
            <div class="flex flex-col card flex-1 text-center py-6 mx-4">
                <div class="text-grey-dark text-sm uppercase text-center font-bold tracking-wider mb-2 md:text-md">Uptime Status</div>
                <span class="flex flex-1 py-2 px-4 font-bold rounded text-center text-lg uppercase items-center justify-center mx-6 my-2 bg-success-light text-success">online</span>
                <div class="text-grey-dark text-xs uppercase text-center font-bold tracking-wider mb-1 md:text-md">Now</div>
            </div>
            <div class="flex flex-col card flex-1 text-center py-6 mx-4">
                <div class="text-grey-dark text-sm uppercase text-center font-bold tracking-wider mb-2 md:text-md">Uptime Status</div>
                <span class="flex flex-1 py-2 px-4 font-bold rounded text-center text-lg uppercase items-center justify-center mx-6 my-2 bg-success-light text-success">online</span>
                <div class="text-grey-dark text-xs uppercase text-center font-bold tracking-wider mb-1 md:text-md">Now</div>
            </div>
            <div class="flex flex-col card flex-1 text-center py-6 mx-4">
                <div class="text-grey-dark text-sm uppercase text-center font-bold tracking-wider mb-2 md:text-md">Uptime Status</div>
                <span class="flex flex-1 py-2 px-4 font-bold rounded text-center text-lg uppercase items-center justify-center mx-6 my-2 bg-success-light text-success">online</span>
                <div class="text-grey-dark text-xs uppercase text-center font-bold tracking-wider mb-1 md:text-md">Now</div>
            </div>
        </div>

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
