<template>
  <div class="footer-top bg-gray-400 text-black dark:text-white">
    <div>
      <vs-row>
        <vs-col w="2" />
        <vs-col w="2">
          <div class="py-8">
            <div class="font-bold text-2xl mb-4">
              <h1>
                Brands
              </h1>
            </div>
            <div>
              <p>
                Adidas
              </p>
              <p>
                Puma
              </p>
              <p>
                Rebook
              </p>
              <p>
                Nike
              </p>
            </div>
          </div>
        </vs-col>
        <vs-col w="2">
          <div class="py-8">
            <div class="font-bold text-2xl mb-4">
              <h1>
                Company
              </h1>
            </div>
            <div>
              <p>
                About us
              </p>
              <p>
                Career
              </p>
              <p>
                Find a store
              </p>
              <p>
                Rules and Terms
              </p>
              <p>
                Sitemap
              </p>
            </div>
          </div>
        </vs-col>
        <vs-col w="2">
          <div class="py-8">
            <div class="font-bold text-2xl mb-4">
              <h1>
                Help
              </h1>
            </div>
            <div>
              <p>
                Contact us
              </p>
              <p>
                Money refund
              </p>
              <p>
                Order Status
              </p>
              <p>
                Shipping info
              </p>
              <p>
                Open Dispute
              </p>
            </div>
          </div>
        </vs-col>
        <vs-col w="2">
          <div class="py-8">
            <div class="font-bold text-2xl mb-4">
              <h1>
                Account
              </h1>
            </div>
            <div>
              <p>
                User Login
              </p>
              <p>
                User Register
              </p>
              <p>
                Account settings
              </p>
              <p>
                My orders
              </p>
            </div>
          </div>
        </vs-col>
        <vs-col w="2">
          <div class="py-8">
            <div class="font-bold text-2xl mb-4">
              <h1>
                Social
              </h1>
            </div>
            <div>
              <p>
                Facebook
              </p>
              <p>
                Twitter
              </p>
              <p>
                Instagram
              </p>
              <p>
                Line
              </p>
            </div>
          </div>
        </vs-col>
      </vs-row>
    </div>
    <div class="footer bg-gray-500 dark:bg-gray-800 dark:text-white text-black">
      <div>
        <img src="~/assets/footer.svg" alt="" class="footer-img mx-auto" />
      </div>
      <div>
        <vs-button-group>
          <vs-button id="switchTheme" border color="success">
            System
          </vs-button>
          <vs-button border color="success">
            Light
          </vs-button>
          <vs-button border color="success">
            Dark
          </vs-button>
        </vs-button-group>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped>

</style>
