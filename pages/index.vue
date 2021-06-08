<template>
  <div>
    <div>
      <TopNav />
      <div class="container mx-auto mb-8 mt-4 text-black bg-white dark:bg-gray-600 dark:text-white p-3 shadow-lg">
        <vs-row>
          <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="2" class="px-5">
            <div class="container bg-green-500 text-center mb-6 p-2">
              <h1>Categories</h1>
            </div>
            <p class="mb-2">
              Electronics
            </p>
            <hr />
            <p class="mb-2">
              Accessories
            </p>
            <hr />
            <p class="mb-2">
              Women's
            </p>
            <hr />
            <p class="mb-2">
              Men's Collection
            </p>
            <hr />
            <p class="mb-2">
              Babies & Toys
            </p>
            <hr />
            <p class="mb-2">
              Home Appliances
            </p>
            <hr />
            <p class="mb-2">
              Motorcycles
            </p>
            <hr />
            <p class="mb-2">
              Electronics
            </p>
            <hr />
            <p class="mb-2">
              Accessories
            </p>
            <hr />
            <p class="mb-2">
              Women's
            </p>
            <hr />
            <p class="mb-2">
              Men's Collection
            </p>
            <hr />
            <p class="mb-2">
              Babies & Toys
            </p>
            <hr />
            <p class="mb-2">
              Home Appliances
            </p>
            <hr />
            <p class="mb-2">
              Motorcycles
            </p>
          </vs-col>
          <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="8">
            <div>
              <img src="~/assets/carousel-1.jpg" alt="" />
            </div>
          </vs-col>
          <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="2" class="px-5">
            <div class="container bg-green-500 text-center mb-10 p-2">
              <h1>Top Categories</h1>
            </div>
            <div class="container">
              <vs-row>
                <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                  <div>
                    <b>
                      Headphone
                    </b>
                  </div>
                  <div>
                    <button>
                      Source
                    </button>
                  </div>
                </vs-col>
                <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                  <div>
                    <vs-card type="2">
                      <template #title>
                        <h3>Pot with a plant</h3>
                      </template>
                      <template #img>
                        <img src="~/assets/items/5.jpg" alt="" />
                      </template>
                    </vs-card>
                  </div>
                </vs-col>
              </vs-row>
              <hr class="py-2 mt-4" />
              <vs-row>
                <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                  <div>
                    <b>
                      Watch
                    </b>
                  </div>
                  <div>
                    <button>
                      Source
                    </button>
                  </div>
                </vs-col>
                <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                  <div>
                    <vs-card type="2">
                      <template #title>
                        <h3>Pot with a plant</h3>
                      </template>
                      <template #img>
                        <img src="~/assets/items/2.jpg" alt="" />
                      </template>
                    </vs-card>
                  </div>
                </vs-col>
              </vs-row>
              <hr class="py-2 mt-4" />
              <vs-row>
                <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                  <div>
                    <b>
                      Mobile
                    </b>
                  </div>
                  <div>
                    <button>
                      Source
                    </button>
                  </div>
                </vs-col>
                <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                  <div>
                    <vs-card type="2">
                      <template #title>
                        <h3>Pot with a plant</h3>
                      </template>
                      <template #img>
                        <img src="~/assets/items/8.jpg" alt="" />
                      </template>
                    </vs-card>
                  </div>
                </vs-col>
              </vs-row>
            </div>
          </vs-col>
        </vs-row>
      </div>
      <div class="container mx-auto text-black bg-white dark:bg-gray-600 dark:text-white p-5 mb-4 shadow-lg">
        <vs-row>
          <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="4">
            <div class="text-4xl font-bold mb-2 pt-5">
              <h1>Deals and Offers</h1>
            </div>
            <div class="mb-3 text-2xl">
              <small>Equipments</small>
            </div>
            <CountdownTimer
              :year="2020"
              :month="8"
              :date="8"
              :hour="12"
              :minute="15"
              :second="59"
              :millisecond="31"
            />
          </vs-col>
          <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="2">
            <vs-card type="2" class="p-4">
              <template #title>
                <h3>Pot with a plant</h3>
              </template>
              <template #img>
                <img src="~/assets/items/1.jpg" alt="" />
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
              </template>
            </vs-card>

            <div class="text-center">
              <h1>Price</h1>
            </div>
            <div class="text-center">
              <h1>-20%</h1>
            </div>
          </vs-col>
          <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="2">
            <vs-card type="2" class="p-4">
              <template #title>
                <h3>Pot with a plant</h3>
              </template>
              <template #img>
                <img src="~/assets/items/11.jpg" alt="" />
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
              </template>
            </vs-card>
            <div class="text-center">
              <h1>Price</h1>
            </div>
            <div class="text-center">
              <h1>-20%</h1>
            </div>
          </vs-col>
          <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="2">
            <vs-card type="2" class="p-4">
              <template #title>
                <h3>Pot with a plant</h3>
              </template>
              <template #img>
                <img src="~/assets/items/10.jpg" alt="" />
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
              </template>
            </vs-card>
            <div class="text-center">
              <h1>Price</h1>
            </div>
            <div class="text-center">
              <h1>-20%</h1>
            </div>
          </vs-col>
          <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="2">
            <vs-card type="2" class="p-4">
              <template #title>
                <h3>Pot with a plant</h3>
              </template>
              <template #img>
                <img src="~/assets/items/9.jpg" alt="" />
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
              </template>
            </vs-card>
            <div class="text-center">
              <h1>Price</h1>
            </div>
            <div class="text-center">
              <h1>-20%</h1>
            </div>
          </vs-col>
        </vs-row>
      </div>
      <div class="container mx-auto">
        <div class="py-6">
          <h1 class="font-bold text-4xl dark:text-white">
            Apparel
          </h1>
        </div>
        <div class="container mx-auto text-black bg-white dark:bg-gray-600 dark:text-white mb-4 shadow-lg">
          <vs-row>
            <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="3" class="summer bg-gradient-to-r from-green-400 to-blue-500 text-white">
              <div class="text-3xl font-bold p-6 mt-5 text-center">
                <h1>
                  Best Products
                </h1>
              </div>
              <div class="p-5">
                <small>
                  It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is t
                </small>
              </div>
              <div class="px-10 my-10">
                <vs-button
                  danger
                  gradient
                  block
                >
                  <i class="bx bxs-conversation"></i> Explore Now
                </vs-button>
              </div>
            </vs-col>
            <vs-col
              vs-type="flex"
              vs-justify="center"
              vs-align="center"
              offset="1"
              w="2"
              class="p-5"
            >
              <div class="text-2xl font-bold">
                <h1 class="font-bold text-2xl">
                  Product Name
                </h1>
              </div>
              <div>
                <vs-row>
                  <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                    <div>
                      <i class="bx bxs-map"></i>
                      <small>Location</small>
                    </div>
                  </vs-col>
                  <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                    <div>
                      <vs-card type="2">
                        <template #title>
                          <h3>Pot with a plant</h3>
                        </template>
                        <template #img>
                          <img src="~/assets/items/3.jpg" alt="" />
                        </template>
                      </vs-card>
                    </div>
                  </vs-col>
                </vs-row>
              </div>
              <div>
                <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="12" class="mt-5">
                  <div class="text-2xl font-bold">
                    <h1 class="font-bold text-2xl">
                      Product Name
                    </h1>
                  </div>
                  <div>
                    <vs-row>
                      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                        <div>
                          <i class="bx bxs-map"></i>
                          <small>Location</small>
                        </div>
                      </vs-col>
                      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                        <div>
                          <vs-card type="2">
                            <template #title>
                              <h3>Pot with a plant</h3>
                            </template>
                            <template #img>
                              <img src="~/assets/items/8.jpg" alt="" />
                            </template>
                          </vs-card>
                        </div>
                      </vs-col>
                    </vs-row>
                  </div>
                </vs-col>
              </div>
            </vs-col>
            <vs-col
              vs-type="flex"
              vs-justify="center"
              vs-align="center"
              offset="1"
              w="2"
              class="p-5"
            >
              <div class="text-2xl font-bold">
                <h1 class="font-bold text-2xl">
                  Product Name
                </h1>
              </div>
              <div>
                <vs-row>
                  <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                    <div>
                      <i class="bx bxs-map"></i>
                      <small>Location</small>
                    </div>
                  </vs-col>
                  <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                    <div>
                      <vs-card type="2">
                        <template #title>
                          <h3>Pot with a plant</h3>
                        </template>
                        <template #img>
                          <img src="~/assets/items/14.jpg" alt="" />
                        </template>
                      </vs-card>
                    </div>
                  </vs-col>
                </vs-row>
              </div>
              <div>
                <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="12" class="mt-5">
                  <div class="text-2xl font-bold">
                    <h1 class="font-bold text-2xl">
                      Product Name
                    </h1>
                  </div>
                  <div>
                    <vs-row>
                      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                        <div>
                          <i class="bx bxs-map"></i>
                          <small>Location</small>
                        </div>
                      </vs-col>
                      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                        <div>
                          <vs-card type="2">
                            <template #title>
                              <h3>Pot with a plant</h3>
                            </template>
                            <template #img>
                              <img src="~/assets/items/12.jpg" alt="" />
                            </template>
                          </vs-card>
                        </div>
                      </vs-col>
                    </vs-row>
                  </div>
                </vs-col>
              </div>
            </vs-col>
            <vs-col
              vs-type="flex"
              vs-justify="center"
              offset="1"
              vs-align="center"
              w="2"
              class="p-5"
            >
              <div class="text-2xl font-bold">
                <h1 class="font-bold text-2xl">
                  Product Name
                </h1>
              </div>
              <div>
                <vs-row>
                  <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                    <div>
                      <i class="bx bxs-map"></i>
                      <small>Location</small>
                    </div>
                  </vs-col>
                  <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                    <div>
                      <vs-card type="2">
                        <template #title>
                          <h3>Pot with a plant</h3>
                        </template>
                        <template #img>
                          <img src="~/assets/items/6.jpg" alt="" />
                        </template>
                      </vs-card>
                    </div>
                  </vs-col>
                </vs-row>
              </div>
              <div>
                <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="12" class="mt-5">
                  <div class="text-2xl font-bold">
                    <h1 class="font-bold text-2xl">
                      Product Name
                    </h1>
                  </div>
                  <div>
                    <vs-row>
                      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                        <div>
                          <i class="bx bxs-map"></i>
                          <small>Location</small>
                        </div>
                      </vs-col>
                      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                        <div>
                          <vs-card type="2">
                            <template #title>
                              <h3>Pot with a plant</h3>
                            </template>
                            <template #img>
                              <img src="~/assets/items/2.jpg" alt="" />
                            </template>
                          </vs-card>
                        </div>
                      </vs-col>
                    </vs-row>
                  </div>
                </vs-col>
              </div>
            </vs-col>
            <vs-col
              vs-type="flex"
              vs-justify="center"
              vs-align="center"
              w="2"
              offset="1"
              class="p-5"
            >
              <div class="text-2xl font-bold">
                <h1 class="font-bold text-2xl">
                  Product Name
                </h1>
              </div>
              <div>
                <vs-row>
                  <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                    <div>
                      <i class="bx bxs-map"></i>
                      <small>Location</small>
                    </div>
                  </vs-col>
                  <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                    <div>
                      <vs-card type="2">
                        <template #title>
                          <h3>Pot with a plant</h3>
                        </template>
                        <template #img>
                          <img src="~/assets/items/7.jpg" alt="" />
                        </template>
                      </vs-card>
                    </div>
                  </vs-col>
                </vs-row>
              </div>
              <div>
                <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="12" class="mt-5">
                  <div class="text-2xl font-bold">
                    <h1 class="font-bold text-2xl">
                      Product Name
                    </h1>
                  </div>
                  <div>
                    <vs-row>
                      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                        <div>
                          <i class="bx bxs-map"></i>
                          <small>Location</small>
                        </div>
                      </vs-col>
                      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="6">
                        <div>
                          <vs-card type="2">
                            <template #title>
                              <h3>Pot with a plant</h3>
                            </template>
                            <template #img>
                              <img src="~/assets/items/1.jpg" alt="" />
                            </template>
                          </vs-card>
                        </div>
                      </vs-col>
                    </vs-row>
                  </div>
                </vs-col>
              </div>
            </vs-col>
          </vs-row>
        </div>
      </div>
      <div class="container mx-auto">
        <div class="py-6">
          <h1 class="font-bold text-4xl dark:text-white">
            Query
          </h1>
        </div>
        <div class="container mx-auto mb-4 shadow-lg">
          <vs-row>
            <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="7">
              <div>
                <img
                  src="~/assets/station.jpeg"
                  alt=""
                />
              </div>
            </vs-col>
            <vs-col
              vs-type="flex"
              vs-justify="center"
              vs-align="center"
              w="5"
              class="text-black bg-white dark:bg-gray-600 dark:text-white p-10 query-box"
            >
              <div class="text-4xl font-bold text-center mt-12 mb-5">
                <h1>
                  One Query, Multiple Products
                </h1>
              </div>
              <div class="center content-inputs px-20 text-black">
                <vs-input placeholder="What are you looking for?" />
              </div>
              <div class="px-20 mb-5 text-black">
                <vs-input
                  type="number"
                  placeholder="Quantity"
                />
              </div>
              <div>
                <div class="mx-20 sample-request">
                  <vs-checkbox>
                    Request For Sample
                  </vs-checkbox>
                  <vs-checkbox>
                    Request For Price
                  </vs-checkbox>
                </div>
              </div>
              <div class="text-black">
                <div class="center content-inputs px-20 my-5">
                  <vs-input placeholder="Details (optional)" />
                </div>
              </div>
              <div class="my-6 px-20">
                <vs-button
                  danger
                  gradient
                  block
                >
                  <i class="bx bxs-conversation"></i> Explore Now
                </vs-button>
              </div>
            </vs-col>
          </vs-row>
        </div>
      </div>
      <div class="container mx-auto mb-4">
        <div class="py-6">
          <h1 class="font-bold text-4xl dark:text-white">
            Recommended Products
          </h1>
        </div>
        <div>
          <vs-row class="mx-20">
            <vs-col
              v-for="(product, index) in products"
              :key="index"
              vs-type="flex"
              vs-justify="center"
              vs-align="center"
              w="2"
              class="mx-3 my-3"
            >
              <InteractualCard :product="product" />
            </vs-col>
          </vs-row>
        </div>
      </div>

      <div class="container mx-auto pt-10">
        <img src="~/assets/banners-long.jpg" alt="" />
      </div>

      <div class="text-center mt-20 bg-gradient-to-r from-green-400 to-blue-500">
        <vs-row>
          <vs-col w="2" />
          <vs-col w="8">
            <div class="pt-8 dark:text-white">
              <h1>
                Delivering the latest product trends and industry news straight to your inbox
              </h1>
              <div class="sample-request justify-center">
                <vs-input
                  type="search"
                  placeholder="Search"
                  class="search-box"
                />
                <vs-button
                  danger
                  gradient
                >
                  <i class="bx bxs-conversation"></i> Subscribe
                </vs-button>
              </div>
              <div class="pb-10">
                <small>We will never share your email with anyone</small>
              </div>
            </div>
          </vs-col>
          <vs-col w="2" />
        </vs-row>
      </div>
    </div>
  </div>
</template>

<script>
import TopNav from '~/components/common/HeaerComponents/TopNav'
import InteractualCard from '~/components/common/InteractualCard'
import CountdownTimer from '~/components/Countdown Timer'
export default {
  name: 'Dashboard',
  components: { CountdownTimer, InteractualCard, TopNav },
  data: () => ({
    products: [
      {
        id: 1,
        name: 'Navy Tea-Shirt',
        img: require('~/assets/items/1.jpg'),
        isFavourite: false,
        rating: '4',
        price: '750.00'
      },
      {
        id: 2,
        name: 'Brown Jacket',
        img: require('~/assets/items/2.jpg'),
        isFavourite: false,
        rating: '4.9',
        price: '1050.00'
      },
      {
        id: 3,
        name: 'Short Pant',
        img: require('~/assets/items/3.jpg'),
        isFavourite: false,
        rating: '4.1',
        price: '350.00'
      },
      {
        id: 4,
        name: 'Shoulder Bag',
        img: require('~/assets/items/4.jpg'),
        isFavourite: false,
        rating: '4',
        price: '45.00'
      },
      {
        id: 5,
        name: 'Apple iMac',
        img: require('~/assets/items/5.jpg'),
        isFavourite: false,
        rating: '3.9',
        price: '135000.00'
      },
      {
        id: 6,
        name: 'Grey Sofa Set',
        img: require('~/assets/items/6.jpg'),
        isFavourite: false,
        rating: '0.0',
        price: '3600.00'
      },
      {
        id: 7,
        name: 'Smart Watch',
        img: require('~/assets/items/7.jpg'),
        isFavourite: false,
        rating: '5.0',
        price: '13000.00'
      },
      {
        id: 8,
        name: 'Ipod',
        img: require('~/assets/items/8.jpg'),
        isFavourite: false,
        rating: '1.6',
        price: '12000.00'
      },
      {
        id: 9,
        name: 'Headset Stereo',
        img: require('~/assets/items/9.jpg'),
        isFavourite: false,
        rating: '2.6',
        price: '2750.00'
      },
      {
        id: 10,
        name: 'Smart Assistant',
        img: require('~/assets/items/10.jpg'),
        isFavourite: false,
        rating: '4.6',
        price: '26000.00'
      }
    ]
  })
}
</script>

<style scoped>

</style>
