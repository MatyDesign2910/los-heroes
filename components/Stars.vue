<template>
  <div>
    <img
      :src="rating"
      class="rating-slider-nuxt"
    />
  </div>
</template>
<script>
export default {
  name: "Stars",
  data() {
      return {
        rating: require('~/assets/img/star.svg'),
      }
  },
    props: {
        datosNavegacion: Object
    }
};
</script>
<style scoped>
</style>