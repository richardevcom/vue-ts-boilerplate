<script setup lang="ts">
defineProps<{
  msg: string;
}>();
</script>

<template>
  <h1 class="text-4xl font-medium -top-2.5 text-center lg:text-left">
    {{ msg }}
  </h1>
  <h3 class="lg:text-left text-xl text-center">
    You’ve successfully created a project with
    <a href="https://vitejs.dev/" class="" target="_blank" rel="noopener"
      >Vite</a
    >
    +
    <a href="https://vuejs.org/" class="" target="_blank" rel="noopener"
      >Vue 3</a
    >. What's next?
  </h3>
</template>
