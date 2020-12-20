<template>
  <router-link
    class="block sm:inline-block sm:px-4 py-2 hover:text-gray-300 transition-colors duration-300 ml-3 sm:ml-0"
    :to="to"
    >{{ label }}</router-link
  >
</template>

<script>
export default {
  props: {
    to: {
      type: String,
      required: true
    },
    label: {
      type: String,
      required: true
    }
  }
};
</script>
