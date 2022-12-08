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
  <h2 v-if="count > 10">count is greater than 10</h2>
  <h2 v-else-if="count > 5">count is greater than 5</h2>
  <h2 v-else>count is less than 5</h2>
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
