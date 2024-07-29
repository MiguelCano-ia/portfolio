<template>
  <div class="flex flex-col items-center bg-gray-800 p-4 rounded-lg shadow-md text-center hover:scale-105 hover:transition-transform transition-transform">
    <img :src="logo" alt="Technology Logo" class="w-16 h-16 mb-2"/>
    <p class="text-white text-lg font-semibold">{{ name }}</p>
  </div>
</template>

<script setup lang="ts">
  interface Props {
   name: string;
   logo: string;
  }

  defineProps<Props>();
</script>