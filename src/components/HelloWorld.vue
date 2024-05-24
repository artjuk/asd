<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <div>count is {{ count }}</div>
    <button type="button" @click="count++">+</button>
    <button type="button" @click="count--">-</button>
  </div>
</template>

<style scoped>
.card > div {
  margin-bottom: 0.5rem;
}
</style>
