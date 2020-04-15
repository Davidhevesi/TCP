<template>
  <Carousel :per-page="1" class="-mt-6">
    <slide>
      <g-image src="~/layouts/img/Car2.jpg" class="h-full" />
    </slide>
    <slide>
      <g-image src="~/layouts/img/Motocycle.jpg" class="h-full" />
    </slide>
    <slide>
      <g-image src="~/layouts/img/Porche.jpg" class="h-full" />
    </slide>
  </Carousel>
</template>

<script>
import { Carousel, Slide } from "vue-carousel";
export default {
  components: {
    Carousel,
    Slide
  }
};
</script>

<style lang="scss" scoped></style>
