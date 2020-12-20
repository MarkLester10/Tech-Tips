<template>
  <div class="relative z-0 h-screen">
    <img
      src="/images/img1.jpg"
      alt="Hero"
      class="block w-full h-full object-cover object-top"
    />
    <div class="absolute inset-0 bg-black opacity-30"></div>
    <div class="px-4 sm:px-0 absolute inset-0 text-white">
      <div
        class="container relative mx-auto h-full flex flex-col justify-center"
      >
        <div class="text-4xl sm:text-6xl font-bold animate-pulse">
          Your Daily Dose of Tech
        </div>
        <div
          class="mt-12 sm:w-1/2 tracking-wider font-roboto font-light text-md sm:text-lg"
        >
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consequuntur
          recusandae eos eum repudiandae distinctio molestias in animi
          laudantium saepe odit voluptatibus maiores, labore optio sit officia,
          ab tempora dolorem ut hic rerum dignissimos! Asperiores est alias
          earum doloremque id reprehenderit itaque unde quisquam doloribus eum,
          ipsam repudiandae ea libero ad?
        </div>
        <img
          src="/images/mouse.gif"
          class="block w-10 absolute bottom-16 left-1/2"
          alt="Scroll"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped></style>
