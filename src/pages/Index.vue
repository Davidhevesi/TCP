<template>
  <Layout>
    <Carousel />
    <FeaturedServices />
  </Layout>
</template>

<script>
import FeaturedServices from "~/components/FeaturedServices.vue";
import Carousel from "~/components/Carousel.vue";

export default {
  data() {
    return {
      /* data properties here */
    };
  },
  components: {
    FeaturedServices,
    Carousel
  }
};
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
