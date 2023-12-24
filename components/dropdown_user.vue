<script setup>
import { Bars3Icon,UserCircleIcon } from '@heroicons/vue/24/solid'
const items = [
  [{
    label: 'Profile',
    avatar: {
      src: 'https://avatars.githubusercontent.com/u/739984?v=4'
    }
  }], [{
    label: 'Edit',
    icon: 'i-heroicons-pencil-square-20-solid',
    shortcuts: ['E'],
    click: () => {
      console.log('Edit')
    }
  }, {
    label: 'Duplicate',
    icon: 'i-heroicons-document-duplicate-20-solid',
    shortcuts: ['D'],
    disabled: true
  }], [{
    label: 'Archive',
    icon: 'i-heroicons-archive-box-20-solid'
  }, {
    label: 'Move',
    icon: 'i-heroicons-arrow-right-circle-20-solid'
  }], [{
    label: 'Delete',
    icon: 'i-heroicons-trash-20-solid',
    shortcuts: ['⌘', 'D']
  }]
]
</script>

<template>
  <UDropdown :items="items" :popper="{ placement: 'bottom-start' }">
    <button class="top-0 right-0 hover:shadow-xl text-white px-4 py-2 rounded-3xl flex items-center space-x-1 border-gray-400 border w-18">
    <Bars3Icon class="w-6 text-gray-600"></Bars3Icon>
    <UserCircleIcon class="w-8 text-gray-600"></UserCircleIcon>
    </button>
  </UDropdown>
</template>

