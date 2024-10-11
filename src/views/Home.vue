<script setup lang="ts">
import { ref } from "vue";
const count = ref(0);
</script>
<template>
  <div class="flex space-x-2">
    <button @click="count++" class="px-4 py-2 bg-blue-500 rounded-md">
      Increment
    </button>
    <p class="text-4xl">
      {{ count }}
    </p>
  </div>
</template>
