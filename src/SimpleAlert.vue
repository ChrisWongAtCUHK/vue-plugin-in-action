<template>
  <p>Well done!</p>
</template>
<script>
import { setTimeout } from 'timers'
export default {
  name: 'SimpleAlert',
  props: {
    message: {
      type: String,
      default: 'Hello Dev.to'
    },
    timeout: {
      type: Number,
      default: 0
    }
  },
  mounted () {
    setTimeout(() => {
      alert(this.message)
    }, this.timeout)
  }
}
</script>
