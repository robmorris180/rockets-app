<template>
  <section class="row">
    <rocket v-for="rocket in rockets" :key="rocket.name" :rocket="rocket"></rocket>
  </section>
</template>

<script>
import Rocket from "@/components/Rocket";
export default {
  name: "rocket-list",
  props: ["rockets"],
  components: {
    Rocket
  }
};
</script>