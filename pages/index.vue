<script setup>
const array = [
{
  name: "John",
  city: "New York",
  country: "USA"
},
{
  name: "Yoshiaki",
  city: "Osaka",
  country: "Japan"
}

]
</script>

<template>
  <AppHeader txtColor="text-indigo-800" text="Different Components" />
  <AppCardContainer bgColor="bg-red-100">
    <AppCard v-for="card in array" :key="card.id" :name="card.name" :city="card.city" :country="card.country" bgColor="bg-slate-300" txtColor="text-indigo-500"></AppCard>
  </AppCardContainer>

  <AppButton bgColor="bg-yellow-500" txtColor="text-black" text="Clickable Button" />
  <AppButton bgColor="bg-red-500" txtColor="text-white" text="Clickable Button 2" />
</template>