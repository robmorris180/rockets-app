<template>
  <section>
    <new-rockets-form></new-rockets-form>
    <rocket-list :rockets="rockets"></rocket-list>
  </section>
</template>

<script>
import NewRocketsForm from "@/components/NewRocketsForm";
import RocketList from "@/components/RocketList";
import API from "@/lib/api";

export default {
  name: "rockets",
  components: {
    NewRocketsForm,
    RocketList
  },
  data: () => ({
    rockets: []
  }),
  async mounted() {
    this.rockets = await API.getRockets();
  }
};
</script>

<style>
</style>