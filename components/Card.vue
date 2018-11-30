<template>
      <div class="card">
        <div v-if="header" class="card--header px-8 py-8 border-b-2 border-grey-lighter">
            <h1 class="text-black uppercase tracking-wider text-base">{{ header }}</h1>
        </div>
        <div class="card--content">
          <slot name="content"></slot>
        </div>
        <div class="card--footer border-t-2 border-grey-lighter px-8">
            <slot name="footer"></slot>
        </div>

      </div>
</template>

<script>
export default {
    props: ['header']
}
</script>

<style>
 .card {
     border-radius: .5rem;
    background-color: #fff;
    -webkit-box-shadow: 0 18px 35px rgba(50,50,93,.1), 0 8px 15px rgba(0,0,0,.07);
    box-shadow: 0 18px 35px rgba(50,50,93,.1), 0 8px 15px rgba(0,0,0,.07);
    overflow: hidden;
 }

.card--header,
.card--footer{
    background: #fbfcfd;
}
</style>
