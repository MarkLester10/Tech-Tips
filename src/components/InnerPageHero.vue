<template>
  <div class="relative z-0 h-40 sm:h-64">
    <img :src="imgUrl" alt="about" class="h-full w-full object-cover" />
    <div class="absolute inset-0 bg-black opacity-50"></div>
    <div
      class="absolute inset-0 bg-gradient-to-t from-gray-900 opacity-90"
    ></div>
    <div class="absolute inset-0 text-white">
      <div
        class="container mx-auto px-4 sm:px-0 h-full w-full flex flex-col items-center justify-center sm:justify-end 
        text-2xl sm:text-5xl"
      >
        <h1 class="sm:mb-8 text-center">{{ title }}</h1>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    imgUrl: {
      type: String,
      required: true,
    },
    title: {
      type: String,
      required: true,
    },
  },
  setup() {
    return {};
  },
};
</script>
