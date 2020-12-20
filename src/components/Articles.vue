<template>
  <div>
    <div
      :class="{
        'space-y-8 sm:space-y-16': isList,
        'space-y-16 sm:space-y-0 grid sm:grid-cols-3 sm:gap-12': isGrid,
      }"
    >
      <Article :layout="layout" />
      <Article :layout="layout" />
      <Article :layout="layout" />
      <Article :layout="layout" />
      <Article :layout="layout" />
      <Article :layout="layout" />
      <Article :layout="layout" />
      <Article :layout="layout" />
      <Article :layout="layout" />
    </div>
    <div v-if="showViewAll" class="mt-8 sm:mt-12">
      <router-link
        to="/articles"
        class="block sm:inline w-full sm:w-auto px-4 sm:px-6 py-4 sm:py-3 text-center bg-red-400 text-white rounded focus:outline-none hover:bg-black transition-colors duration-300 shadow-md"
        >View All</router-link
      >
    </div>
  </div>
</template>

<script>
import Article from "@/components/Article";
import { computed } from "vue";

export default {
  props: {
    layout: {
      type: String,
      default: "list",
    },
    showViewAll: {
      type: Boolean,
      default: true,
    },
  },
  components: {
    Article,
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

<style lang="scss" scoped></style>
