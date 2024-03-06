<template>
  <div class="card">
    <h2>{{ Destination.name }}</h2>
    <img :src="Destination.img" alt="" />
    <h3>{{ clicked }}</h3>
    <button>Click Me</button>
  </div>
</template>

<script setup>
import { ref } from "vue";
//const emit = defineEmits(["BtnClick"]);

//emit("BtnClick", Destination);
const props = defineProps({
  Destination: Object,
});

//clicker logic
const clicked = ref(0);
function increment() {
  clicked.value++;
}
</script>

<style scoped>
img {
  width: 300px;
  height: 350px;
  object-fit: cover;
}
button {
  width: 150px;
  height: 200px;
}
.card {
  width: 24%;
}
</style>
