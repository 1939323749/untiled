<script setup>
import Button from './components/Button.vue'
import Test from "@/components/Test.vue";
</script>

<template>
  <header>

    <div class="wrapper">

    </div>
  </header>

  <body>
  <div id="app">
    <Button/>
  </div>
  <div>
    <Test/>
  </div>


  </body>
</template>

<style scoped>
header {
  line-height: 1.5;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
