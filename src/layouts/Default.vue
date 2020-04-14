<template>
  <div class="max-w-screen-2xl m-auto">
    <header class="bg-gray-900 mb-6 sm:flex sm:justify-between sm:">
      <div class="flex justify-between bg-gray-900 px-4 py-3 mr-10">
        <span
          class="shadow-outline px-1 py-1 font-semibold text-xl tracking-tight text-gray-100"
        >
          <g-link class="m-2 mr text-white" to="/">{{
            $static.metadata.siteName
          }}</g-link></span
        >
        <div class="flex sm:hidden">
          <button
            @click="isOpen = !isOpen"
            type="button"
            class="px-2 text-gray-500 hover:text-white focus:outline-none focus:text-white border rounded"
          >
            <svg
              class="h-6 w-6 fill-current"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
            >
              <path
                v-if="isOpen"
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M18.278 16.864a1 1 0 0 1-1.414 1.414l-4.829-4.828-4.828 4.828a1 1 0 0 1-1.414-1.414l4.828-4.829-4.828-4.828a1 1 0 0 1 1.414-1.414l4.829 4.828 4.828-4.828a1 1 0 1 1 1.414 1.414l-4.828 4.829 4.828 4.828z"
              />
              <path
                v-if="!isOpen"
                fill-rule="evenodd"
                d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"
              />
            </svg>
          </button>
        </div>
      </div>
      <nav
        :class="isOpen ? 'block' : 'hidden'"
        class="px-2 pt-2 pb-5 sm:block sm:flex mt-2 mr-10"
      >
        <g-link
          class="nav__link text-white block  rounded hover:bg-gray-800"
          to="/about/"
          >About</g-link
        >

        <g-link
          class="nav__link text-white block rounded hover:bg-gray-800"
          to="/services/"
          >Services</g-link
        >
        <g-link
          class="nav__link text-white block rounded hover:bg-gray-800"
          to="/portfolio/"
          >Portfolio</g-link
        >
        <g-link
          class="nav__link text-white rounded block hover:bg-gray-800"
          to="/faqs/"
          >FAQ'S</g-link
        >
        <g-link
          class="nav__link text-white block rounded hover:bg-gray-800"
          to="/contact/"
          >Contact</g-link
        >
      </nav>
    </header>
    <slot />
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>
body {
  font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.5;
}

.layout {
  max-width: 760px;
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
}

.nav__link {
  margin-left: 20px;
}
</style>
<script>
export default {
  prop: [],
  data() {
    return {
      isOpen: false
    };
  },
  methods: {
    toggle() {
      this.isOpen = !this.isOpen;
    }
  }
};
</script>
