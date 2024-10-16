<script setup lang="ts">
defineProps({
  color: {
    type: String,
    default: "#3bb77e",
  },
  hoverColor: {
    type: String,
    default: "#2b7a4b",
  },
});
</script>
<template>
  <div class="flex">
    <button
      :class="[
        'flex',
        'items-center',
        'justify-center',
        'gap-3',
        'px-6',
        'py-3',
        'rounded-md',
        'text-white',
        'custom-background-color',
        'custom-hover-background-color',
      ]"
    >
      Shop Now
      <img src="./images/right-arrow-7359.svg" alt="right arrow" class="w-5" />
    </button>
  </div>
</template>
<style scoped>
.custom-background-color {
  background-color: v-bind(color);
}

.custom-hover-background-color:hover {
  background-color: v-bind(hoverColor);
}
</style>
