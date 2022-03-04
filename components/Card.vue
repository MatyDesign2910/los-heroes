<template>
  <div class="container-card">
    <NuxtLink :to="datosNavegacion.link_url">
      <div class="card-img">
        <img v-bind:src="datosNavegacion.item_photo" class="img-slider-nuxt" />
      </div>
      <div class="d-flex">
        <div class="card-title">
          <h4>{{ datosNavegacion.location }}</h4>
        </div>
        <div class="card-rating">
          <template v-for="itemStar in datosNavegacion.stars">
            <Stars
              :key="itemStar" :value="itemStar"
            />
          </template>
        </div>
      </div>
      <div class="d-flex">
        <div class="card-description">
          <p>{{ datosNavegacion.hotel_name }}</p>
        </div>
        <div class="card-price">
          <p>{{ datosNavegacion.price }}</p>
        </div>
      </div>
    </NuxtLink>
  </div>
</template>
<script>
export default {
  name: "Cards",
  data() {
    return {
      imgCard: require("~/assets/img/sea_travel_1920.png"),
      rating: require("~/assets/img/star.svg"),
    };
  },
  props: {
    datosNavegacion: Object,
  },
};
</script>
<style scoped>
</style>