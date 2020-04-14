<template>
  <Layout>
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
    <div class="">
      <h1 class="text-center">featured services</h1>
    </div>

    <div class="flex flex-col mb-4 md:flex md:flex-row">
      <div class="md:w-1/2 h-12 md:ml-12 mb-20">
        <div class="px-2 py-2">
          <h1 class="text-center">COLOR CHANGE VINYL WRAPS</h1>
          <p class="text-center px-2 py-2">
            Full single color or customized vinyl wrapping services for cars,
            bikes and boats.
          </p>
          <div class="text-center">
            <span class="inline-flex rounded-md shadow-sm">
              <button
                type="button"
                class=" mb-4 inline-flex items-center px-4 py-2 border border-gray-300 text-sm leading-5 font-medium rounded-md text-gray-700 bg-white hover:text-gray-500 focus:outline-none focus:border-blue-300 focus:shadow-outline-blue active:text-gray-800 active:bg-gray-50 transition ease-in-out duration-150"
              >
                More Details
              </button>
            </span>
          </div>
        </div>
      </div>
      <div class="md:w-1/2 h-12">
        <div class="md:w-1/2 h-12 md:ml-12">
          <div class="">
            <h1 class="text-center">COLOR CHANGE VINYL WRAPS</h1>
            <p class="text-center">
              Full single color or customized vinyl wrapping services for cars,
              bikes and boats.
            </p>
            <div class="text-center">
              <span class="inline-flex rounded-md shadow-sm">
                <button
                  type="button"
                  class="inline-flex items-center px-4 py-2 border border-gray-300 text-sm leading-5 font-medium rounded-md text-gray-700 bg-white hover:text-gray-500 focus:outline-none focus:border-blue-300 focus:shadow-outline-blue active:text-gray-800 active:bg-gray-50 transition ease-in-out duration-150"
                >
                  More Details
                </button>
              </span>
            </div>
          </div>
        </div>
      </div>
      <div class="md:w-1/2 bg-gray-600 h-12">
        <div class="md:w-1/2 h-12 md:ml-12">
          <div class="">
            <h1 class="text-center">COLOR CHANGE VINYL WRAPS</h1>
            <p class="text-center">
              Full single color or customized vinyl wrapping services for cars,
              bikes and boats.
            </p>
            <div class="text-center">
              <span class="inline-flex rounded-md shadow-sm">
                <button
                  type="button"
                  class="inline-flex items-center px-4 py-2 border border-gray-300 text-sm leading-5 font-medium rounded-md text-gray-700 bg-white hover:text-gray-500 focus:outline-none focus:border-blue-300 focus:shadow-outline-blue active:text-gray-800 active:bg-gray-50 transition ease-in-out duration-150"
                >
                  More Details
                </button>
              </span>
            </div>
          </div>
        </div>
      </div>
      <div class="md:w-1/2 h-12 mr-12">
        <div class="md:w-1/2 h-12 md:ml-12">
          <div class="">
            <h1 class="text-center">COLOR CHANGE VINYL WRAPS</h1>
            <p class="text-center">
              Full single color or customized vinyl wrapping services for cars,
              bikes and boats.
            </p>
            <div class="text-center">
              <span class="inline-flex rounded-md shadow-sm">
                <button
                  type="button"
                  class="inline-flex items-center px-4 py-2 border border-gray-300 text-sm leading-5 font-medium rounded-md text-gray-700 bg-white hover:text-gray-500 focus:outline-none focus:border-blue-300 focus:shadow-outline-blue active:text-gray-800 active:bg-gray-50 transition ease-in-out duration-150"
                >
                  More Details
                </button>
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </Layout>
</template>

<script>
import { Carousel, Slide } from "vue-carousel";

export default {
  data() {
    return {
      /* data properties here */
    };
  },
  components: {
    Carousel,
    Slide
  }
};
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
