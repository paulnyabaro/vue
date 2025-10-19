<script setup lang="ts">

import { ref } from 'vue'

const items = ref([
  "10 party hats",
  "2 board games",
  "20 cups"
])

</script>

<template>
  <ul v-if="items">
    <li v-for="(item, index) in items" :key="index">{{ index }}. {{ item }}</li>
  </ul>
</template>

<style scoped></style>
