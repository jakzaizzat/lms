<template>
      <div class="card">
        <div v-if="header" class="card--header px-8 py-8 border-b-2 border-grey-lighter">
            <h1 class="text-black uppercase tracking-wider text-base">{{ header }}</h1>
        </div>
        <div class="card--content">
          <slot name="content"></slot>
        </div>
      </div>
</template>

<script>
export default {
    props: ['header']
}
</script>

<style>
.card--header{
    background: #fbfcfd;
}
</style>
