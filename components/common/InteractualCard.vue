<template>
  <vs-card>
    <template #title>
      <div class="interaction">
        <h3>{{ product.name }}</h3>
        <div class="btn-cart">
          <vs-button
            icon
            relief
            warn
            gradient
            animation-type="rotate"
          >
            <i class="bx bx-cart-alt"></i>
          </vs-button>
        </div>
      </div>
    </template>
    <template #img>
      <img :src="product.img" :alt="product.name" />
    </template>
    <template #text>
      <div class="interaction">
        <b>
          {{ product.price }}
        </b>
        <div>
          <i class="bx bxs-star"></i>
          <i class="bx bxs-star"></i>
          <i class="bx bxs-star"></i>
          <i class="bx bxs-star"></i>
          <i class="bx bxs-star"></i>
        </div>
      </div>
    </template>
    <template #interactions>
      <div class="interaction">
        <vs-button
          icon
          relief
          danger
          animation-type="rotate"
        >
          <i class="bx bx-heart"></i>
          <template #animate>
            <i class="bx bxs-heart"></i>
          </template>
        </vs-button>
        <vs-button class="btn-chat" shadow primary>
          <i class="bx bx-chat"></i>
          <span class="span">
            54
          </span>
        </vs-button>
      </div>
    </template>
  </vs-card>
</template>

<script>
export default {
  name: 'InteractualCard',
  props: {
    product: {
      type: Object,
      required: true
    }
  }
}
</script>

<style scoped>

</style>
