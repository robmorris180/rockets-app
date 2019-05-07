<template>
  <section id="app">
    <nav-bar></nav-bar>
    <rockets class="container mt-4"></rockets>
  </section>
</template>

<script>
import Rockets from "@/views/Rockets.vue";
import NavBar from "@/components/NavBar.vue";

export default {
  name: "app",
  components: {
    Rockets,
    NavBar
  }
};
</script>

<style>
</style>
