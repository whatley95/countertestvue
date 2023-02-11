<!-- <template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style> -->


<template>
  <div class="about">
    <h1>C1 Val</h1>
    <button class="counter-button" @click="storeCounter.increaseCount">
      {{ storeCounter.count }}
    </button>
  </div>
</template>

<script setup>
import { useCounterStore } from '@/stores/counter'

const storeCounter = useCounterStore()
</script>

<style>
.counter-button {
  font-size: 60px;
}
</style>