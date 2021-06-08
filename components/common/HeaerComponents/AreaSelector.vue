<template>
  <div class="center">
    <div>
      <p class="inline-flex pr-3 text-white" style="font-size: 22px">
        <i class="bx bxs-map text-3xl text-white mr-3" @click="showAreaModal=!showAreaModal"></i>
        {{ areaValue }}
      </p>
    </div>
    <vs-dialog
      v-model="showAreaModal"
      width="300px"
      not-center
      not-close
      prevent-close
      blur
    >
      <template #header>
        <h4 class="not-margin text-center">
          Please Select Your Current <b>Area</b>
        </h4>
      </template>

      <div class="center">
        <vs-select v-model="areaValue" placeholder="Select">
          <template #message-danger>
            Required
          </template>
          <vs-option label="Barisal" value="Barisal">
            Barisal
          </vs-option>
          <vs-option label="Chittagong" value="Chittagong">
            Chittagong
          </vs-option>
          <vs-option label="Dhaka" value="Dhaka">
            Dhaka
          </vs-option>
          <vs-option label="Khulna" value="Khulna">
            Khulna
          </vs-option>
          <vs-option label="Mymensingh" value="Mymensingh">
            Mymensingh
          </vs-option>
          <vs-option label="Rajshahi" value="Rajshahi">
            Rajshahi
          </vs-option>
          <vs-option label="Rangpur" value="Rangpur">
            Rangpur
          </vs-option>
          <vs-option label="Sylhet" value="Sylhet">
            Sylhet
          </vs-option>
        </vs-select>
      </div>

      <template #footer>
        <div class="con-footer">
          <vs-button block transparent @click="showAreaModal=false">
            Submit
          </vs-button>
        </div>
      </template>
    </vs-dialog>
  </div>
</template>

<script>
export default {
  name: 'AreaSelector',
  data: () => ({
    areaValue: '',
    showAreaModal: false
  }),
  mounted () {
    if (!this.areaValue) {
      this.showAreaModal = !this.showAreaModal
    }
  }
}
</script>

<style scoped>

</style>
