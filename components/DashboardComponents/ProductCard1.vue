<template>
  <div class="container text-center mx-auto">
    <b class="product-heading text-gray-600">
      Recent Products
    </b>
    <vs-card-group>
      <vs-card class="shadow-lg">
        <template #title>
          <h3>Pot with a plant</h3>
        </template>
        <template #img>
          <img src="~/assets/p1.jpeg" alt="" @click="activeProduct=!activeProduct" />
        </template>
        <template #text>
          <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit.
          </p>
        </template>
        <template #interactions>
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
        </template>
      </vs-card>
    </vs-card-group>
    <div class="center">
      <vs-dialog v-model="activeProduct" overflow-hidden blur>
        <template #header>
          <h4 class="not-margin">
            Welcome to <b class="brand-name">Shopify</b>
          </h4>
        </template>

        <vs-row>
          <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
            <div>
              <img src="~/assets/p1.jpeg" alt="" />
            </div>
          </vs-col>
          <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
            <div>
              <div class="mb-3">
                <b>Product Name</b>
              </div>
              <div class="mb-3">
                <vs-row>
                  <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="8">
                    <p>Product Description</p>
                  </vs-col>
                  <vs-col vs-type="flex" vs-justify="flex-end" vs-align="right" w="4">
                    <vs-row>
                      <i class="bx bxs-star"></i>
                      <i class="bx bxs-star"></i>
                      <i class="bx bxs-star"></i>
                      <i class="bx bxs-star"></i>
                      <i class="bx bxs-star"></i>
                    </vs-row>
                  </vs-col>
                </vs-row>
                <hr />
              </div>
              <div class="mb-5">
                <small>
                  Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old. Richard McClintock, a Latin professor at Hampden-Sydney College in Virginia, looked up one of the more obscure Latin words, consectetur, from a Lorem Ipsum passage, and going through the cites of the word in classical literature, discovered the undoubtable source. Lorem Ipsum comes from sections 1.10.32 and 1.10.33 of "de Finibus Bonorum et Malorum" (The Extremes of Good and Evil) by Cicero, written in 45 BC. This book is a treatise on the theory of ethics, very popular during the Renaissance. The first line of Lorem Ipsum, "Lorem ipsum dolor sit amet..", comes from a line in section 1.10.32.
                </small>
              </div>
              <vs-row>
                <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="3">
                  <vs-button
                    gradient
                    style="min-width: 150px"
                    warn
                    animation-type="scale"
                    block
                  >
                    <i class="bx bxs-shopping-bag"></i>
                    <template #animate>
                      Add to Cart
                    </template>
                  </vs-button>
                </vs-col>
                <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="4">
                  <vs-button
                    gradient
                    style="min-width: 150px"
                    success
                    animation-type="scale"
                    block
                  >
                    <i class="bx bxs-cart-download" style="color:#ffffff"></i>
                    <template #animate>
                      Buy Now
                    </template>
                  </vs-button>
                </vs-col>
                <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="3">
                  <vs-button
                    gradient
                    style="min-width: 150px"
                    danger
                    animation-type="scale"
                    block
                  >
                    <i class="bx bxs-bookmark-alt-plus" style="color:#ffffff"></i>
                    <template #animate>
                      Favourite
                    </template>
                  </vs-button>
                </vs-col>
              </vs-row>
            </div>
          </vs-col>
        </vs-row>
      </vs-dialog>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ProductCard1',
  data: () => ({
    activeProduct: false
  })
}
</script>

<style scoped>

</style>
