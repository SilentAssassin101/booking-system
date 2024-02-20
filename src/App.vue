<script>
import { /*RouterLink,*/ RouterView } from 'vue-router'
import MainNavbar from './components/MainNavbar.vue'
import DaisyAlert from './components/DaisyAlert.vue';

export default {
  components: {
    MainNavbar,
    RouterView,
    DaisyAlert
  }
}
</script>

<template>
  <header class="sticky z-40 top-0">
    <MainNavbar />
    <DaisyAlert type="warning" text="Warning: This site is still heavily a work in progress!"
      class="bg-warning text-black" />
  </header>
  <main>
    <RouterView />
  </main>
</template>

<style></style>
