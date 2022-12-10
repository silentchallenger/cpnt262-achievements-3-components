<script setup>
defineProps({
  txtColor: {
    type: String,
    default: "text-black"
  },
  text: {
    type: String,
    default: "Default Heading"
  }
})
</script>

<template>
  <h1 :class="txtColor" class="text-2xl p-4">{{ text }}</h1>
</template>