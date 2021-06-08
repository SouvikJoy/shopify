<template>
  <div class="center">
    <i class="bx bx-cart-alt text-3xl text-white mr-3" @click="showCart = !showCart">
      <vs-dialog v-model="showCart" width="300px" not-center>
        <template #header>
          <h4 class="not-margin text-center">
            You have no products in your cart
          </h4>
        </template>

        <template #footer>
          <div class="con-footer">
            <vs-button block dark transparent @click="showCart=false">
              Cancel
            </vs-button>
          </div>
        </template>
      </vs-dialog>
    </i>
  </div>
</template>

<script>
export default {
  name: 'Cart',
  data: () => ({
    showCart: false
  })
}
</script>

<style scoped>

</style>
