<template>
  <div>
    <header>
      <Header />
    </header>
    <main>
      <Nuxt />
    </main>
    <footer>
      <Footer />
    </footer>
  </div>
</template>

<script>
import Header from '~/components/common/Header'
import Footer from '~/components/common/Footer'

export default {
  name: 'Shopify',
  components: {
    Header,
    Footer
  }
}
</script>

<style lang="scss">
header {
  height: 64px;
}
</style>
