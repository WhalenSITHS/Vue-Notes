<template>
  <div>
    <h1 v-if="test === true">Good</h1>
    <h1 v-else>Bad</h1>
    <h2 v-for="animal in animals" :key="animal">{{ animal }}</h2>
  </div>
</template>

<script setup>
const animals = ["zebra", "camel", "ape"];
const test = false;
</script>

<style scoped></style>
