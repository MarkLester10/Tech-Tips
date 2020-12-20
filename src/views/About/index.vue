<template>
  <InnerPageHero imgUrl="/images/team.jpg" title="About us" />
  <div class="container px-4 sm:px-0 mx-auto py-8 sm:py-12 mb-16">
    <div class="grid sm:grid-cols-5 gap-2 sm:gap-12">
      <div class="sm:col-span-3 h-64 sm:h-400 shadow-lg">
        <img
          src="/images/team2.jpg"
          alt="Hero"
          class="w-full h-full object-cover"
        />
        <div
          class="px-3 py-3 text-base sm:text-2xl text-white bg-black text-center"
        >
          We can make impossible, possible
        </div>
      </div>
      <div class="sm:col-span-2">
        <div class="font-roboto mt-20 sm:mt-2 text-lg text-gray-700">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Cumque,
          illum modi consequatur blanditiis, amet facere odit quos nostrum,
          architecto dicta eveniet quibusdam voluptatibus! Nihil, alias facere
          excepturi unde voluptatem necessitatibus. Lorem ipsum dolor sit amet
          consectetur adipisicing elit. Perspiciatis excepturi est, consequuntur
          odio tenetur placeat rerum, blanditiis ratione sed reiciendis enim
          aperiam, unde distinctio quasi dicta quos. Doloribus vel consequatur
          id ea deserunt tempore magnam, eligendi eos architecto quisquam,
          reprehenderit necessitatibus maiores numquam explicabo veniam
          accusamus, minus quo itaque. Fugit? Lorem100
        </div>
      </div>
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

<style lang="scss" scoped></style>
