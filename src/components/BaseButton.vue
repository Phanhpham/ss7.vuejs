<template>
  <button>
    <slot></slot>
  </button>
</template>

<script setup>
const props = defineProps({
  title: {
    default: "Click me 1",
    type: String,
    required: true,
  },
});
console.log("Props:", props);
</script>

<style></style>
