<script setup>
defineProps({
  bgColor: {
    type: String,
    default: "bg-red-300"
  }
})
</script>

<template>
  <div class="flex flex-row p-4 gap-6" :class="bgColor">
    <slot></slot>
  </div>
</template>