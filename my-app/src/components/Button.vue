<script setup>
import { ref } from 'vue'

let count = ref(0)
function increment() {
  count.value++
}

</script>

<template>
  <button @click="increment" class="rounded bg-gray-800 p-4 text-white hover:bg-gray-700 cursor-pointer
          transition-transform duration-100 ease-out
          hover:scale-104 
          active:scale-96">
    {{ `Counter: ` + count }}
  </button>
</template>