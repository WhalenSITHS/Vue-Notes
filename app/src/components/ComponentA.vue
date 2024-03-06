<!-- ComponentA.vue -->
<script setup>
import { store } from "../stores/store";
</script>

<template>
  <button @click="store.count++">From B: {{ store.count }}</button>
</template>
<style scoped>
button {
  width: 200px;
  height: 150px;
  font-size: 25px;
}
</style>
