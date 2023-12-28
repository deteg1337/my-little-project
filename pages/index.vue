<script setup lang="ts">
definePageMeta({
  layout: 'navbar'
})
</script>

<template>
  <CategoryBar></CategoryBar>
  <HSpacer></HSpacer>
  <div class="flex flex-col">
    <div class="flex flex-row justify-between">
      <v-spacer></v-spacer>
      <HousingCard />
      <HousingCard />
      <HousingCard />
      <HousingCard />
      <v-spacer></v-spacer>
    </div>
    <h-spacer></h-spacer>
    <div class="flex flex-row justify-between">
      <v-spacer></v-spacer>
      <HousingCard />
      <HousingCard />
      <HousingCard />
      <HousingCard />
      <v-spacer></v-spacer>
    </div>
  </div>
</template>
