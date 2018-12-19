<template>
    <div class="w-full max-w-screen mx-auto px-4">
        <div class="flex py-3 border-b border-grey">
            <div class="flex flex-1">
                <Logo></Logo>
            </div>
            <div class="flex justify-between items-center">
                <ul class="list-reset flex">
                    <li>
                        <nuxt-link to="/home" class="flex items-center no-underline text-grey-darker group hover:text-black ml-10">
                            <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="fill-current w-6 h-6 mr-2 group-hover:text-primary text-grey-dark"><path d="M4 14h4v-4H4v4zm0 5h4v-4H4v4zM4 9h4V5H4v4zm5 5h12v-4H9v4zm0 5h12v-4H9v4zM9 5v4h12V5H9z"></path> <path d="M0 0h24v24H0z" fill="none"></path></svg>
                            <span class="font-medium text-grey-darker">User Dashboard</span>
                        </nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="/admin" class="flex items-center no-underline text-grey-darker group hover:text-black ml-10">
                            <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="fill-current w-6 h-6 mr-2 group-hover:text-primary text-grey-dark"><path d="M4 14h4v-4H4v4zm0 5h4v-4H4v4zM4 9h4V5H4v4zm5 5h12v-4H9v4zm0 5h12v-4H9v4zM9 5v4h12V5H9z"></path> <path d="M0 0h24v24H0z" fill="none"></path></svg>
                            <span class="font-medium text-grey-darker">Admin Dashboard</span>
                        </nuxt-link>
                    </li>
                    <li>
                        <nuxt-link to="/leave/apply" class="flex items-center no-underline text-grey-darker group hover:text-black ml-10">
                            <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="fill-current w-6 h-6 mr-2 group-hover:text-primary text-grey-dark"><path d="M4 14h4v-4H4v4zm0 5h4v-4H4v4zM4 9h4V5H4v4zm5 5h12v-4H9v4zm0 5h12v-4H9v4zM9 5v4h12V5H9z"></path> <path d="M0 0h24v24H0z" fill="none"></path></svg>
                            <span class="font-medium text-grey-darker">{{ loggedInUser }}</span>
                        </nuxt-link>
                    </li>
                </ul>
                <div class="flex items-center ml-6 pl-6 border-l border-grey">
                    <img src="https://secure.gravatar.com/avatar/6b401b039d76ecd311a274f63dcde958?s=35&amp;r=g&amp;d=identicon" width="35" height="35" class="rounded-full">
                    <div class="ml-3 flex-1">
                        <div class="text-black text-sm font-bold leading-tight">Jakz Aizzat</div>
                        <a href="https://pingping.io/logout" class="text-primary hover:underline text-sm font-bold leading-tight no-underline block">Log out</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>


<script>
import { mapGetters } from 'vuex'
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
  computed: {
    ...mapGetters(['isAuthenticated', 'loggedInUser'])
  }
}
</script>

<style>
    .nuxt-link-active svg{
        color: #2b79c1;
    }
    .nuxt-link-active span{
        color: #1b476f;
        font-weight: bold;
    }
</style>
