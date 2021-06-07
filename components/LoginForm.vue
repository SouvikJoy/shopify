<template>
  <div>
    <vs-button
      block
      color="rgb(59,222,200)"
      gradient
      @click="active = !active"
    >
      Sign In
    </vs-button>
    <vs-dialog
      id="div-with-loading"
      v-model="active"
      class="vs-con-loading__container"
      blur
      prevent-close
    >
      <template #header>
        <h2 class="not-margin login-form-title">
          Welcome to <b class="brand-name">Shopify</b>
        </h2>
      </template>

      <div class="con-form">
        <vs-input v-model="email" placeholder="john@email.com">
          <template #icon>
            @
          </template>
          <template v-if="validEmail" #message-success>
            Email Valid
          </template>
          <template v-if="!validEmail && email !== ''" #message-danger>
            Email Invalid
          </template>
        </vs-input>
        <vs-input v-model="password" type="password" placeholder="Password">
          <template #icon>
            <i class="bx bxs-lock"></i>
          </template>
        </vs-input>
        <div class="flex">
          <vs-checkbox v-model="remember">
            Remember me
          </vs-checkbox>
          <a href="#">Forgot Password?</a>
        </div>
      </div>

      <template #footer>
        <div class="footer-dialog">
          <vs-button
            block
            color="rgb(59,222,200)"
            gradient
            @click="signIn"
          >
            Sign In
          </vs-button>

          <div class="text-center new">
            New Here? <a href="#">Create New Account</a>
          </div>
        </div>
      </template>
    </vs-dialog>
  </div>
</template>
<script>
export default {
  name: 'LoginForm',
  data: () => ({
    active: false,
    email: '',
    password: '',
    remember: false,
    user: null
  }),
  computed: {
    validEmail () {
      return /^\w+([.-]?\w+)*@\w+([.-]?\w+)*(\.\w{2,3})+$/.test(this.email)
    }
  },
  /* mounted () {
    if (!this.user) {
      this.active = !this.active
      const loading = this.$vs.loading()
      setTimeout(() => {
        loading.close()
      }, 3000)
    }
  }, */
  methods: {
    signIn () {
      this.$router.push('/')

      this.$vs.notification({
        color: 'success',
        title: 'Login Successfully Done',
        text: `These documents refer to the latest version,
            to see the documents of the previous versions you can do it here 👉`
      })

      const loading = this.$vs.loading()
      setTimeout(() => {
        loading.close()
      }, 2000)

      console.log('Logged In', this.email, this.password)
    }
  }
}
</script>

<style scoped>

</style>
