<template>
  <InnerPageHero imgUrl="/images/img1.jpg" title="Article Title" />
  <div class="container px-4 sm:px-0 mx-auto py-8 sm:py-12 mb-16">
    <div
      class="flex flex-col sm:flex-row space-y-2 sm:space-y-0 sm:items-center justify-between flex-wrap text-base"
    >
      <div class="flex items-center text-gray-600">
        <div>
          <svg
            class="w-4 h-4"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M7 7h.01M7 3h5c.512 0 1.024.195 1.414.586l7 7a2 2 0 010 2.828l-7 7a2 2 0 01-2.828 0l-7-7A1.994 1.994 0 013 12V7a4 4 0 014-4z"
            ></path>
          </svg>
        </div>
        <div class="ml-1">Category Name</div>
      </div>

      <div class="flex items-center text-gray-600">
        <div>
          <svg
            class="w-4 h-4"
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
        </div>
        <div class="ml-1 text-sm">
          September 18th, 2020
        </div>
      </div>
    </div>

    <div class="mt-6 sm:mt-12">
      <p class="mt-4">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Numquam,
        magni? Quae voluptatibus vitae odio at neque. Exercitationem qui non
        aspernatur vel, deleniti sapiente minima laudantium ex eos iusto harum
        repudiandae corporis fugiat dolorum earum magnam, maiores quaerat
        corrupti a vitae delectus explicabo. Omnis deleniti quos maiores, veniam
        ratione eos aut.
      </p>
      <p class="mt-4">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Numquam,
        magni? Quae voluptatibus vitae odio at neque. Exercitationem qui non
        aspernatur vel, deleniti sapiente minima laudantium ex eos iusto harum
        repudiandae corporis fugiat dolorum earum magnam, maiores quaerat
        corrupti a vitae delectus explicabo. Omnis deleniti quos maiores, veniam
        ratione eos aut.
      </p>
      <p class="mt-4">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Numquam,
        magni? Quae voluptatibus vitae odio at neque. Exercitationem qui non
        aspernatur vel, deleniti sapiente minima laudantium ex eos iusto harum
        repudiandae corporis fugiat dolorum earum magnam, maiores quaerat
        corrupti a vitae delectus explicabo. Omnis deleniti quos maiores, veniam
        ratione eos aut.
      </p>
      <p class="mt-4">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Numquam,
        magni? Quae voluptatibus vitae odio at neque. Exercitationem qui non
        aspernatur vel, deleniti sapiente minima laudantium ex eos iusto harum
        repudiandae corporis fugiat dolorum earum magnam, maiores quaerat
        corrupti a vitae delectus explicabo. Omnis deleniti quos maiores, veniam
        ratione eos aut.
      </p>
    </div>
  </div>
</template>

<script>
import InnerPageHero from "@/components/InnerPageHero";

export default {
  components: {
    InnerPageHero,
  },
};
</script>
