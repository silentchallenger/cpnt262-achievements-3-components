<script setup>
defineProps({
  name: {
    type: String,
    default: "Default Name"
  },
  city: {
    type: String,
    default: "Default City"
  },
  country: {
    type: String,
    default: "Default Country"
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
  <section class="border-2 p-4" :class="bgColor">
    <h2 :class="txtColor">{{ name }}</h2>
    <p :class="txtColor">{{ city }}</p>
    <p :class="txtColor">{{ country }}</p>
  </section>
</template>