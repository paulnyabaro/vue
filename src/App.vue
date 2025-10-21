<script setup lang="ts">

import { reactive } from 'vue'

const items = reactive([
  "10 party hats",
  "2 board games",
  "20 cups"
])

</script>

<template>
  <ul v-if="items">
    <li v-for="(item, index) in items" :key="index">{{ index + 1 }}. {{ item }} +</li>
  </ul>
  <!-- <li v-for="n in 100" :key="n" style="display: inline-block;">{{ n }}</li> -->
</template>

<style scoped>
ul{
  background-color: green;
  list-style: none;
  display: flex;
  gap: 1rem;
  padding: 1rem;

  li{
    background-color: #fff3;
    border: 1px solid #fff8;
    padding: 1rem;
    color: #fff;

  }
}
</style>
