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
                                    <svg viewBox="0 0 24 24" class="fill-current w-6 h-6 mr-3 group-hover:text-primary text-grey-dark"><path d="M0 0h24v24H0z" fill="none"></path> <path d="M19.35 10.04A7.49 7.49 0 0 0 12 4C9.11 4 6.6 5.64 5.35 8.04A5.994 5.994 0 0 0 0 14c0 3.31 2.69 6 6 6h13c2.76 0 5-2.24 5-5 0-2.64-2.05-4.78-4.65-4.96z"></path></svg> <span>Details</span>
                                </a>
                            </li>
                            <li>
                                <a href="https://pingping.io/monitors/608/statistics" class="flex items-center no-underline text-grey-darker group hover:text-black py-2">
                                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="fill-current w-6 h-6 mr-3 group-hover:text-primary text-primary"><path d="M5 9.2h3V19H5zM10.6 5h2.8v14h-2.8zm5.6 8H19v6h-2.8z"></path> <path fill="none" d="M0 0h24v24H0z"></path></svg>
                                    <span class="font-bold text-black">Statistics</span>
                                </a>
                            </li>
                            <li>
                                <a href="https://pingping.io/monitors/608/statuspage" class="flex items-center no-underline text-grey-darker group hover:text-black py-2">
                                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="fill-current w-6 h-6 mr-3 group-hover:text-primary text-grey-dark"><path fill="none" d="M0 0h24v24H0z"></path> <path d="M20 19.59V8l-6-6H6c-1.1 0-1.99.9-1.99 2L4 20c0 1.1.89 2 1.99 2H18c.45 0 .85-.15 1.19-.4l-4.43-4.43c-.8.52-1.74.83-2.76.83-2.76 0-5-2.24-5-5s2.24-5 5-5 5 2.24 5 5c0 1.02-.31 1.96-.83 2.75L20 19.59zM9 13c0 1.66 1.34 3 3 3s3-1.34 3-3-1.34-3-3-3-3 1.34-3 3z"></path></svg> <span>Statuspage</span>
                                </a>
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
