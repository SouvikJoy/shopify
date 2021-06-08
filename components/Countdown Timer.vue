<template>
  <div>
    <vs-row>
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="2" class="m-2">
        <div class="container bg-black dark:bg-white dark:text-black text-white p-5 text-center text-4xl rounded-2xl">
          {{ displayDays }}
        </div>
        <div class="text-center">
          Days
        </div>
      </vs-col>
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="2" class="m-2">
        <div class="container bg-black dark:bg-white dark:text-black text-white p-5 text-center text-4xl rounded-2xl">
          {{ displayHours }}
        </div>
        <div class="text-center">
          Hours
        </div>
      </vs-col>
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="2" class="m-2">
        <div class="container bg-black text-white dark:bg-white dark:text-black p-5 text-center text-4xl rounded-2xl">
          {{ displayMinutes }}
        </div>
        <div class="text-center">
          Minutes
        </div>
      </vs-col>
      <vs-col vs-type="flex" vs-justify="center" vs-align="center" w="2" class="m-2">
        <div class="container bg-black text-white dark:bg-white dark:text-black p-5 text-center text-4xl rounded-2xl">
          {{ displaySeconds }}
        </div>
        <div class="text-center">
          Seconds
        </div>
      </vs-col>
    </vs-row>
    <h5 v-if="!expired">
      Hop in now for this exciting offer!! Don't be lazy...
    </h5>
    <h5 v-else>
      Offer Expired! Don't be late next time..
    </h5>
  </div>
</template>

<script>
export default {
  name: 'CountdownTimer',
  props: {
    year: {
      type: Number,
      required: true
    },
    month: {
      type: Number,
      required: true
    },
    date: {
      type: Number,
      required: true
    },
    hour: {
      type: Number,
      required: true
    },
    minute: {
      type: Number,
      required: true
    },
    second: {
      type: Number,
      required: true
    },
    millisecond: {
      type: Number,
      required: true
    }
  },
  data () {
    return {
      displayDays: 0,
      displayHours: 0,
      displayMinutes: 0,
      displaySeconds: 0,
      loaded: false,
      expired: false
    }
  },
  computed: {
    _seconds: () => 1000,
    _minutes () {
      return this._seconds * 60
    },
    _hours () {
      return this._minutes * 60
    },
    _days () {
      return this._hours * 24
    },
    end () {
      return new Date(
        this.year,
        this.month,
        this.date,
        this.hour,
        this.minute,
        this.second,
        this.millisecond
      )
    }
  },
  mounted () {
    this.showRemaining()
  },
  methods: {
    formatNum: num => (num < 10 ? '0' + num : num),

    showRemaining () {
      const timer = setInterval(() => {
        const now = new Date()

        const distance = this.end.getTime() - now.getTime()
        if (distance < 0) {
          clearInterval(timer)
          this.expired = true
          this.loaded = true
          return
        }
        const days = Math.floor(distance / this._days)
        const hours = Math.floor((distance % this._days) / this._hours)
        const minutes = Math.floor((distance % this._hours) / this._minutes)
        const seconds = Math.floor((distance % this._minutes) / this._seconds)

        this.displayDays = this.formatNum(days)
        this.displayHours = this.formatNum(hours)
        this.displayMinutes = this.formatNum(minutes)
        this.displaySeconds = this.formatNum(seconds)
        this.loaded = true
      }, 1000)
    }
  }
}
</script>

<style scoped>

</style>
