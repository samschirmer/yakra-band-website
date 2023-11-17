<script setup>
import { RouterView } from 'vue-router'
import MainNavbar from './components/MainNavbar.vue';
import PageFooter from './components/PageFooter.vue';
</script>

<template>
  <MainNavbar />

  <RouterView />

  <PageFooter />
</template>

<style scoped>

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) { }
</style>
