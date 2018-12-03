<template>
    <div class="bg-primary-lightest font-serif relative border-t-8 border-primary min-h-screen py-4">
        <div class="container mx-auto px-6">
            <Nav/>
            <div class="flex-1">
                <div class="w-full max-w-screen mx-auto px-4 flex py-8">
                    <div class="hidden lg:block lg:w-1/6 mr-8">
                        <ul class="list-reset mb-8">
                            <div class="pb-3 font-bold uppercase text-black">Epal Valley</div>
                            <li>
                                <a href="https://pingping.io/monitors/608" class="flex items-center no-underline text-grey-darker group hover:text-black py-2">
                                    <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="fill-current w-6 h-6 mr-2 group-hover:text-primary text-grey-dark"><path d="M12 12c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm0 2c-2.67 0-8 1.34-8 4v2h16v-2c0-2.66-5.33-4-8-4z"></path> <path d="M0 0h24v24H0z" fill="none"></path></svg> <span>User</span>
                                </a>
                            </li>
                            <li>
                                <a href="https://pingping.io/monitors/608/statistics" class="flex items-center no-underline text-grey-darker group hover:text-black py-2">
                                    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="24" height="24" class="fill-current w-6 h-6 text-grey-dark mr-3 group-hover:text-primary text-grey-dark"><defs><path id="a" d="M0 0h24v24H0V0z"></path></defs> <clipPath id="b"><use xlink:href="#a" overflow="visible"></use></clipPath> <path clip-path="url(#b)" d="M14 10H2v2h12v-2zm0-4H2v2h12V6zM2 16h8v-2H2v2zm19.5-4.5L23 13l-6.99 7-4.51-4.5L13 14l3.01 3 5.49-5.5z"></path></svg>
                                    <span class="font-bold text-black">History</span>
                                </a>
                            </li>
                            <li>
                                <a href="https://pingping.io/monitors/608/statuspage" class="flex items-center no-underline text-grey-darker group hover:text-black py-2">
                                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="fill-current w-6 h-6 mr-3 group-hover:text-primary text-grey-dark"><path fill="none" d="M0 0h24v24H0z"></path> <path d="M20 19.59V8l-6-6H6c-1.1 0-1.99.9-1.99 2L4 20c0 1.1.89 2 1.99 2H18c.45 0 .85-.15 1.19-.4l-4.43-4.43c-.8.52-1.74.83-2.76.83-2.76 0-5-2.24-5-5s2.24-5 5-5 5 2.24 5 5c0 1.02-.31 1.96-.83 2.75L20 19.59zM9 13c0 1.66 1.34 3 3 3s3-1.34 3-3-1.34-3-3-3-3 1.34-3 3z"></path></svg> <span>Statuspage</span>
                                </a>
                            </li>
                            <li>
                                <nuxt-link to="/leave/apply" class="flex justify-center items-center no-underline text-white text-center bg-primary group font-bold rounded py-2 mt-4">
                                    <span>Apply Leave</span>
                                </nuxt-link>
                            </li>
                        </ul>
                    </div>
                    <div class="flex-1">
                        <nuxt/>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Nav from '~/components/Nav.vue'

export default {
  components: {
    Logo,
    Nav
  }
}
</script>

<style>
html {
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    text-rendering: optimizeLegibility;
}
</style>
