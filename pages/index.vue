<template>
  <div class="container mx-auto px-6 py-16 sm:py-16 md:py-24">
    <div class="mx-auto max-w-sm">
      <div class="py-10 text-center">
        <logo/>
      </div>
      <Card>
        <template slot="content">
          <div class="p-8">
            <h1 class="uppercase text-base font-semibold tracking-wide text-center pb-8 text-blue-darkest">
              Welcome Back
            </h1>

            <label class="block uppercase tracking-wide text-grey-darker text-xs font-bold mb-2" for="grid-first-name">
              Email
            </label>
            <input class="appearance-none block w-full bg-grey-lighter text-grey-darker rounded py-3 px-4 mb-3 leading-tight focus:outline-none" id="grid-first-name" type="email">


            <label class="block uppercase tracking-wide text-grey-darker text-xs font-bold mb-2" for="grid-first-name">
              Password
            </label>
            <input class="appearance-none block w-full bg-grey-lighter text-grey-darker rounded py-3 px-4 mb-3 leading-tight focus:outline-none" id="grid-first-name" type="password">


            <button class="shadow rounded bg-primary text-white uppercase w-full p-4 tracking-wider text-sm my-4">
              log in
            </button>
          </div>
        </template>

        <template slot="footer">
          <div class="flex justify-between py-8">
            <a class="font-medium text-primary hover:text-primary-dark no-underline" href="#">Don't have account yet</a>
            <a class="text-grey-darkest hover:text-black no-underline" href="#">Forgot Password</a>
          </div>
        </template>
      </Card>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Card from '~/components/Card.vue'

export default {
  components: {
    Logo,
    Card
  }
}
</script>
