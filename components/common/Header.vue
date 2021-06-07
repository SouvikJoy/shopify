<template>
  <div>
    <vs-navbar v-model="active" center-collapsed>
      <template #left>
        <img src="~/assets/logo.svg" alt="" class="header-logo" />
      </template>
      <vs-navbar-group>
        <NuxtLink to="#">
          Categories
        </NuxtLink>
        <template #items>
          <vs-navbar-item id="guide" :active="active === 'guide'">
            <NuxtLink to="#">
              Guide
            </NuxtLink>
          </vs-navbar-item>
          <vs-navbar-item id="docs" :active="active === 'docs'">
            <NuxtLink to="#">
              Documents
            </NuxtLink>
          </vs-navbar-item>
          <vs-navbar-item id="components" :active="active === 'components'">
            <NuxtLink to="#">
              Components
            </NuxtLink>
          </vs-navbar-item>
        </template>
      </vs-navbar-group>

      <vs-navbar-item id="1" :active="active === '1'">
        <NuxtLink to="#">
          Documents
        </NuxtLink>
      </vs-navbar-item>
      <vs-navbar-item id="2" :active="active === '2'">
        <NuxtLink to="#">
          Components
        </NuxtLink>
      </vs-navbar-item>
      <vs-navbar-item id="3" :active="active === '3'">
        <NuxtLink to="#">
          license
        </NuxtLink>
      </vs-navbar-item>

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
