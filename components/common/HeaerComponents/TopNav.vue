<template>
  <div class="top-nav bg-white dark:bg-gray-700 dark:border-transparent dark:text-white border text-center text-xl py-2">
    <vs-row>
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="1" />
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="1" />
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="1">
        <div>
          <NuxtLink to="#">
            Top sellers
          </NuxtLink>
        </div>
      </vs-col>
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="1">
        <div>
          <NuxtLink to="#">
            Ready to ship
          </NuxtLink>
        </div>
      </vs-col>
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="1">
        <div>
          <NuxtLink to="#">
            Services
          </NuxtLink>
        </div>
      </vs-col>
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="1">
        <div>
          <NuxtLink to="#">
            Sell with us
          </NuxtLink>
        </div>
      </vs-col>
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="1" />
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="1" />
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="1">
        Get the app
      </vs-col>
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="1">
        English
      </vs-col>
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="1" />
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="1" />
    </vs-row>
  </div>
</template>

<script>
export default {
  name: 'TopNav'
}
</script>

<style scoped>
.topNav {
  margin-top: 64px;
}
</style>
