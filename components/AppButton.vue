<script setup>
defineProps({
  text: {
    type: String,
    default: "Default Text"
  },
  bgColor: {
    type: String,
    default: "bg-red-300"
  },
  txtColor: {
    type: String,
    default: "text-black"
  }
})
</script>

<template>
  <button class="p-4 m-4" :class="bgColor, txtColor">
    {{ text }}
    <slot></slot>
  </button>
</template>