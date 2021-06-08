<template>
  <div>
    <vs-navbar v-model="active" center-collapsed>
      <template #left>
        <img src="~/assets/logo.svg" alt="" class="header-logo" />
        <div class="pl-20 ml-20">
          <NuxtLink to="#" class="font-black">
            CATEGORIES
          </NuxtLink>
        </div>
      </template>

      <vs-input
        type="search"
        placeholder="Search"
        class="search-box"
      />

      <template #right>
        <AreaSelector />
        <Cart />

        <vs-navbar-group>
          <vs-avatar>
            <template #text>
              Sally Willis
            </template>
          </vs-avatar>
          <template #items>
            <vs-avatar size="110">
              <template #text>
                Sally Willis
              </template>
            </vs-avatar>
            <vs-navbar-item>
              <NuxtLink to="#">
                Profile
              </NuxtLink>
            </vs-navbar-item>
            <vs-navbar-item @click="signOut">
              Log Out
            </vs-navbar-item>
          </template>
        </vs-navbar-group>
      </template>
    </vs-navbar>
  </div>
</template>

<script>
import AreaSelector from '~/components/common/HeaerComponents/AreaSelector'
import Cart from '~/components/common/HeaerComponents/Cart'
export default {
  name: 'Header',
  components: {
    AreaSelector,
    Cart
  },
  data: () => ({
    active: 'guide',
    value1: '',
    value2: '',
    valid: {
      email: false,
      password: false
    }
  }),
  methods: {
    signOut () {
      const loading = this.$vs.loading()
      setTimeout(() => {
        loading.close()
      }, 1000)
      this.$vs.notification({
        color: 'danger',
        title: 'Logout Successfully Done',
        text: `These documents refer to the latest version,
            to see the documents of the previous versions you can do it here 👉`
      })
      console.log('Signed out')
      this.$router.push('/')
    }
  }
}
</script>

<style scoped lang="scss">

</style>
