<template>
  <div id="app">
    <TheHeader />
    <TheContent />
    <TheFooter />
  </div>
</template>
<script>
import "@/assets/css/main.css";
export default {
  name: "IndexPage",
  data() {
    return {
      head: {
        link: [{ rel:"stylesheet", type:"text/css", href:'https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@5.15.4/css/fontawesome.min.css' }]
      },
    };
  },
};
</script>
