<template>
    <div class="slider-nuxt">
        <template v-for="mai of main_photo">
            <img :src="mai" class="img-slider-nuxt" />
        </template>
    </div>
</template>
<script>
export default {
    name: "Slider",
    data() {
      return {
        main_photo: []
      }
    },
    async fetch() {
      this.main_photo = await fetch(
        'https://test-desarrollador-front.cclh.io/home/'
      ).then(res => res.json())
    }
};
</script>
<style scoped>

</style>