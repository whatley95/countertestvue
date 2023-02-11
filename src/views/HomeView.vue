<!-- <script setup>
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <main>
    <TheWelcome />
  </main>
</template> -->

<template>
  <div class="home">
    <Counter />
    <div class="button">
      <button @click="storeCounter.decreaseCount">-</button>
      <button @click="storeCounter.increaseCount">+</button>
    </div>
    <hr>
    <div>
      This Counter Is : {{ storeCounter.evenOdd }}
    </div>
    <hr>
    <div>
      <h3>Edit Counter : </h3>
      <input type="number" v-model="storeCounter.count">
    </div>
  </div>
</template>

<script setup>
//import { ref, computed } from 'vue'
import Counter from '@/components/counter/counter.vue'
import { useCounterStore } from '@/stores/counter'

const storeCounter = useCounterStore()

// const count = ref(0)

// const increaseCount = () => {
//   count.value++;
// }

// const decreaseCount = () => {
//   count.value--;
// }

// const evenOdd = computed(() => {
//   if (count.value % 2 === 0) return 'Even'
//   return 'Odd'
// })

</script>

<style>
.count {
  font-size: 70px;
  margin: 25px;
}

.button button {
  font-size: larger;
  margin: 20px;
  width: 100px;
}
</style>
