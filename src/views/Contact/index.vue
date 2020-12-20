<template>
  <InnerPageHero imgUrl="/images/contact.jpg" title="Contact Us" />
  <div class="container px-4 sm:px-0 mx-auto py-8 sm:py-12">
    <div class="grid sm:grid-cols-3 gap-3 sm:gap-4 sm:py-8 text-lg">
      <div>
        <span class="text-gray-500">Address:</span> Lorem ipsum dolor sit amet
      </div>
      <div><span class="text-gray-500">Phone:</span> +123456789</div>
      <div><span class="text-gray-500">Email:</span> Loremipsum@email.com</div>
    </div>

    <div class="mt-8 sm:mt-16 grid sm:grid-cols-2 sm:gap-12">
      <div>
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d25852.25803365898!2d121.11308227379459!3d14.215434063745235!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x33bd63010855c31d%3A0xea95ddf2cffe4cd6!2sCamp%20General%20Vicente%20Lim!5e1!3m2!1sen!2sph!4v1607487847116!5m2!1sen!2sph"
          class="w-full"
          height="450"
          frameborder="0"
          style="border:0;"
          allowfullscreen=""
          aria-hidden="false"
          tabindex="0"
        ></iframe>
      </div>
      <form class="p-8 bg-gray-100 shadow-lg mt-5 sm:mt-0 space-y-4">
        <div>
          <label class="text-gray-400 block mb-2">Full Name</label>
          <input
            type="text"
            class="px-4 py-2 w-full border-2 focus:border-gray-300 focus:outline-none rounded bg-gray-200"
            required
          />
          <!-- <small class="text-xs text-red-400">Error message</small> -->
        </div>
        <div>
          <label class="text-gray-400 block mb-2">Email</label>
          <input
            type="text"
            class="px-4 py-2 w-full border-2 focus:border-gray-300 focus:outline-none rounded bg-gray-200"
            required
          />
          <!-- <small class="text-xs text-red-400">Error message</small> -->
        </div>

        <div>
          <label class="text-gray-400 block mb-2">Message</label>
          <textarea
            rows="5"
            class="px-4 py-2 w-full border-2 focus:border-gray-300 focus:outline-none rounded bg-gray-200"
            required
          ></textarea>
          <!-- <small class="text-xs text-red-400">Error message</small> -->
        </div>

        <!-- <div class="px-4 py-2 bg-green-500 text-white">
          Lorem ipsum dolor sit amet consectetur.
        </div>
        <div class="px-4 py-2 bg-red-400 text-white">
          Lorem ipsum dolor sit amet consectetur.
        </div> -->

        <button
          class="block w-full sm:w-auto px-4 sm:px-6 focus:outline-none hover:bg-black py-4 sm:py-3 transition-colors rounded bg-red-400 text-white"
        >
          Submit
        </button>
      </form>
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
