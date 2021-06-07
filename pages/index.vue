<template>
  <div>
    <Slogan />
    <Services />
    <ProductCard1 />
  </div>
</template>

<script>
import Slogan from '~/components/DashboardComponents/Slogan'
import ProductCard1 from '~/components/DashboardComponents/ProductCard1'
import Services from '~/components/DashboardComponents/Services'
export default {
  name: 'Dashboard',
  components: { Services, ProductCard1, Slogan }
}
</script>

<style scoped>

</style>
