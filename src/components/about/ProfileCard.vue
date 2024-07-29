<template>
  <div class="flex flex-col md:flex-row items-center bg-gray-900 text-white p-6 rounded-lg shadow-lg">
    <div>
      <h2 class="text-4xl font-bold text-gray-300">{{ name }}</h2>
      <p class="mt-4">{{ description }}</p>
    </div>
  </div>
</template>

<script setup lang="ts">
  interface Props {
    name: string;
    description: string;
  }

  defineProps<Props>();
</script>