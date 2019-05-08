<template>
  <section id="app">
    <nav-bar></nav-bar>
    <rockets class="container mt-4"></rockets>
  </section>
</template>

<script>
import NavBar from "@/components/NavBar";
import Rockets from "@/views/Rockets";

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
