<script setup lang="ts">
import { ref } from 'vue'
defineProps<{
  msg: string
}>()
const header = ref('Components List')
</script>

<template>
  <div class="greetings">
    <h2 class="green">{{ header }}</h2>
    <input v-model="header">
    <h3>
      The open source components framework
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
