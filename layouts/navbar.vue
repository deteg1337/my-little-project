<script>
import Dropdown from "/components/dropdown_user.vue";

export default {
  components: {
    Dropdown,
  },
};
</script>

<template>
  <div class="flex justify-between items-center h-20 ml-20 mr-20">
    <HomeIcon class="text-black w-12"></HomeIcon>
    <button class="text-black font-semibold">Filter</button>
    <!-- <Dropdown/> -->
    <DropdownUser class="text-black"></DropdownUser>
  </div>
  <h-spacer></h-spacer>
  <slot></slot>
</template>

<script setup>
import { HomeIcon } from '@heroicons/vue/24/solid'
</script>