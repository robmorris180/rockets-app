<template>
  <section>
    <new-rockets-form></new-rockets-form>
  </section>
</template>

<script>
import NewRocketsForm from "@/components/NewRocketsForm.vue";
import API from "@/lib/api";

export default {
  name: "rockets",
  components: {
    NewRocketsForm
  },
  data: () => ({
    rockets: []
  }),
  async mounted() {
    const rockets = await API.getRockets();
    console.log(rockets);
  }
};
</script>

<style>
</style>