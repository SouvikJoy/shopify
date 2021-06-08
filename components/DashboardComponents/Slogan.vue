<template>
  <div class="background-img" :style="{ backgroundImage: `url(${require('~/assets/carousel-9.jpg')})` }">
    <h1 class="text-center text-4xl font-extrabold text-gray-900 pt-20">
      <span class="block xl:inline">Data To Enrich Your</span>
      <span class="block text-white xl:inline">Online Business</span>
    </h1>
    <p class="mt-3 text-center text-white">
      Qui irure qui lorem cupidatat commodo. Elit sunt amet fugiat veniam occaecat fugiat aliqua.
    </p>
    <p class="mt-3 text-center text-white">
      Anim aute id magna aliqua ad ad non deserunt sunt
    </p>
    <div class="mt-5 mb-6 sm:flex sm:justify-center">
      <div class="rounded-md">
        <vs-button
          danger
          gradient
        >
          <i class="bx bx-shopping-bag"></i> Shop Now
        </vs-button>
      </div>
      <div class="rounded-md pb-20">
        <vs-button
          success
          gradient
        >
          <i class="bx bxs-conversation"></i> Contact us
        </vs-button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Slogan'
}
</script>

<style scoped>
.background-img {
  background-repeat: no-repeat;
  width: auto;
  background-size: cover;
}
</style>
