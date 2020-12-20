<template>
  <div
    class="fixed inset-0 w-full h-full bg-black z-10 opacity-50"
    :class="{ hidden: !isVisible }"
    @click="toggle"
  ></div>
  <button
    class="text-red-400 fixed bottom-10 right-10 z-10 active:outline-none focus:outline-none transform transition-all duration-500"
    :class="{ 'translate-x-72': !showDarkBg }"
    @click="toTop"
  >
    <svg
      class="sm:w-12 sm:h-12 w-8 h-8"
      fill="none"
      stroke="currentColor"
      viewBox="0 0 24 24"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        stroke-linecap="round"
        stroke-linejoin="round"
        stroke-width="1.5"
        d="M8 7l4-4m0 0l4 4m-4-4v18"
      ></path>
    </svg>
  </button>
  <nav
    id="nav"
    class="px-4 py-4 sm:py-5 transition-colors duration-500 bg-transparent fixed w-full z-10"
    :class="{ 'shadow shadow-none bg-black': showDarkBg }"
  >
    <div
      class="container mx-auto flex flex-col sm:flex-row items-center justify-between"
    >
      <div class="w-full flex flex-row items-center justify-between">
        <div>
          <router-link to="/">
            <img src="@/assets/logo.png" class="w-20 sm:w-24" alt="Logo" />
          </router-link>
        </div>
        <div class="sm:hidden">
          <button v-show="!isVisible" @click="toggle" class="flex">
            <svg
              class="w-6 h-6 text-white"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16m-7 6h7"
              ></path>
            </svg>
          </button>
          <button v-show="isVisible" class="flex" @click="toggle">
            <svg
              class="w-6 h-6 text-white"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M6 18L18 6M6 6l12 12"
              ></path>
            </svg>
          </button>
        </div>
      </div>
      <div
        class="mt-4 sm:mt-0 w-full sm:space-x-4 sm:text-right sm:block text-white bg-black sm:bg-transparent
        rounded-md sm:rounded-none p-6 sm:p-0"
        :class="{ hidden: !isVisible }"
      >
        <NavbarLink @click="toggle" to="/" label="Home" />
        <NavbarLink @click="toggle" to="/articles" label="Articles" />
        <NavbarLink @click="toggle" to="/about" label="About" />
        <NavbarLink @click="toggle" to="/contact" label="Contact" />
      </div>
    </div>
  </nav>
</template>

<script>
import NavbarLink from "@/components/layouts/NavbarLink";
import { menuToggle } from "@/composables/userToggle";
import { ref } from "vue";
export default {
  components: {
    NavbarLink,
  },
  props: {},
  setup() {
    let { isVisible, toggle } = menuToggle();
    let showDarkBg = ref(false);

    document.addEventListener("scroll", function() {
      let bodyTopPos = document.body.getBoundingClientRect().top;

      if (bodyTopPos < -150) {
        showDarkBg.value = true;
      } else {
        showDarkBg.value = false;
      }
    });

    function toTop() {
      document.body.scrollTop = 0; // For Safari
      document.documentElement.scrollTop = 0; // For Chrome, Firefox, IE and Opera
    }

    return {
      isVisible,
      toggle,
      showDarkBg,
      toTop,
    };
  },
};
</script>
