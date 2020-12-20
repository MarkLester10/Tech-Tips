<template>
  <div :class="{ 'grid sm:grid-cols-5 gap-2 sm:gap-12': isList }">
    <div
      class="h-64 "
      :class="{ 'sm:h-400 sm:col-span-3': isList, 'sm:col-span-5': isGrid }"
    >
      <img
        src="/images/hero.jpg"
        alt="Hero"
        class="w-full h-full object-cover"
      />
    </div>
    <div class="mt-3 sm:col-span-2 flex flex-col justify-between">
      <div :class="{ 'sm:py-2 sm:mt-0': isGrid }">
        <div class="text-md text-gray-500">
          Category Name
        </div>
        <h3 class="mt-1 leading-tight text-2xl">
          <router-link
            to="/articles/article-slug"
            class="hover:text-red-400 transition-colors duration-300 italic"
            >Lorem ipsum dolor sit amet consectetur adipisicing.</router-link
          >
        </h3>
        <div class="font-roboto mt-2 text-md text-gray-700">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Cumque,
          illum modi consequatur blanditiis, amet facere odit quos nostrum,
          architecto dicta eveniet quibusdam voluptatibus! Nihil, alias facere
          excepturi unde voluptatem necessitatibus ...
        </div>
      </div>
      <div class="mt-1 text-base text-gray-400 flex items-center sm:text-sm">
        <svg
          class="w-5 h-5 mr-2"
          fill="none"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"
          ></path>
        </svg>
        5 mins ago
      </div>
    </div>
  </div>
</template>

<script>
import { computed } from "vue";
export default {
  props: {
    layout: {
      type: String,
      default: "list",
    },
  },
  setup(props) {
    let isGrid = computed(() => {
      return props.layout === "grid";
    });

    let isList = computed(() => {
      return props.layout === "list";
    });
    return {
      isGrid,
      isList,
    };
  },
};
</script>
