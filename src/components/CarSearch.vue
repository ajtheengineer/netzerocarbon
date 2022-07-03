<script setup lang="ts">
import { ref } from "vue";
let input = ref("");
const cars = ["Prius Prime", "Prius", "Tesla", "Rav 4 Prime"];
function filteredList() {
  return cars.filter((car) =>
    car.toLowerCase().includes(input.value.toLowerCase())
  );
}
</script>

<template>
  <input type="text" v-model="input" placeholder="Search cars..." />
  <div class="item car" v-for="car in filteredList()" :key="car">
    <p>{{ car }}</p>
  </div>
  <div class="item error" v-if="input&&!filteredList().length">
     <p>No results found!</p>
  </div>
</template>