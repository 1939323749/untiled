<script>
export default {
  data() {
    return {
      count: 1
    }
  },
  methods: {
    increment() {
      this.count++
    },
    decrement() {
      this.count--
    },
    double() {
      this.count *= 2
    },
    reset() {
      this.count = 1
    }
  }
}
</script>

<template>
  <h1 @click="reset">count: {{ count }}</h1>
  <div id="button">
    <button @click="increment">Increment</button>
    <button @click="decrement">Decrement</button>
    <button @click="double">Double</button>
  </div>
</template>

<style scoped>
button {
  font-weight: bold;
}
</style>
