<template>
  <section class="col-sm-6">
    <div class="card mb-4 rocket">
      <img :src="rocket.image" class="card-img-top rocket__img" :alt="rocket.name">
      <div class="card-body">
        <h5 class="card-title">{{rocket.name}}</h5>
        <h6 class="card-subtitle mb-2 text-muted">{{rocket.country}}</h6>
        <p class="card-text">{{rocket.description}}</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props: ["rocket"]
};
</script>

<style scoped>
.rocket__img {
  height: 400px;
  width: auto;
  margin: 0 auto;
}
</style>
