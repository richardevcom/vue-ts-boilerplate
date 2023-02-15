<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
import LogoSVG from "./components/svg/LogoSVG.vue";
</script>

<template>
  <header class="lg:flex place-items-center max-h-screen pr-20 leading-8">
    <LogoSVG alt="Vue logo" class="lg:m-0 lg:mr-8 block mx-auto mt-0" />

    <div class="lg:flex lg:place-items-start lg:flex-wrap">
      <HelloWorld msg="You did it!" />

      <nav
        class="lg:text-left lg:-ml-4 lg:text-base lg:px-0 lg:py-4 lg:mt-4 w-full mt-8 text-xs text-center"
      >
        <RouterLink
          class="first-of-type:border-0 inline-block px-4 py-0 border border-l border-gray-600"
          to="/"
          >Home</RouterLink
        >
        <RouterLink
          class="first-of-type:border-0 inline-block px-4 py-0 border border-l border-gray-600"
          to="/about"
          >About</RouterLink
        >
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped lang="scss">
nav a {
  &.router-link-exact-active {
    @apply text-gray-800 dark:text-white;

    &:hover {
      @apply bg-transparent;
    }
  }
}
</style>
