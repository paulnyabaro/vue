<script setup>
    import ref from 'vue'

    const value = ref(0)
</script>

<template>
    <button @click="value++">The value is {value}</button>
</template>