<template>
  <InnerPageHero imgUrl="/images/articles.jpg" title="Articles" />
  <div class="container px-4 sm:px-0 mx-auto py-8 sm:py-12 mb-16">
    <Articles layout="grid" :show-view-all="false" />
    <div class="mt-8 sm:mt-12">
      <button
        class="block w-full sm:w-auto px-4 sm:px-6 focus:outline-none hover:bg-black py-4 sm:py-3 transition-colors rounded bg-red-400 text-white"
      >
        Load More
      </button>
    </div>
  </div>
</template>

<script>
import InnerPageHero from "@/components/InnerPageHero";
import Articles from "@/components/Articles";
export default {
  components: {
    InnerPageHero,
    Articles,
  },
};
</script>

<style lang="scss" scoped></style>
