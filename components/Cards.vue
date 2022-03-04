<template>
  <div class="container-cards-row">
    <Card
      v-bind:datosNavegacion="items"
      v-for="items of recommended"
      :key="items"
    />
  </div>
</template>
<script>
export default {
  name: "Cards",
  data() {
    return {
      recommended: [
        {
          item_photo:
            "https://test-desarrollador-front.cclh.io/wp-content/uploads/2022/02/rio_home.png",
          location: "Rio de janeiro",
          hotel_name: "Hotel Boutique Garota",
          stars: "5",
          price: " USD$ 1,260",
          link_url: "/destinos/rio-de-janeiro",
        },
        {
          item_photo:
            "https://test-desarrollador-front.cclh.io/wp-content/uploads/2022/02/punta.png",
          location: "Punta Cana",
          hotel_name: "Resort Ocean Blue",
          stars: "4",
          price: "USD$ 1,320",
          link_url: "/destinos/punta-cana",
        },
        {
          item_photo:
            "https://test-desarrollador-front.cclh.io/wp-content/uploads/2022/02/riviera_home.png",
          location: "Riviera Maya",
          hotel_name: "Riu",
          stars: "5",
          price: "USD$ 1,648",
          link_url: "/destinos/riviera-maya",
        },
        {
          item_photo:
            "https://test-desarrollador-front.cclh.io/wp-content/uploads/2022/02/buenos_home.png",
          location: "Buenos Aires",
          hotel_name: "Hotel Boutique La Rua",
          stars: "3",
          price: " USD$ 1,260",
          link_url: "/destinos/buenos-aires/",
        },
        {
          item_photo:
            "https://test-desarrollador-front.cclh.io/wp-content/uploads/2022/02/san_home.png",
          location: "San Andr\u00e9s",
          hotel_name: "Resort Decameron",
          stars: "4",
          price: "USD$ 1,120",
          link_url: "/destinos/san-andres/",
        },
      ],
    };
  },
};
</script>
<style scoped>
</style>