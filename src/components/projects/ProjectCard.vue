<template>
  <div class="max-w-sm rounded overflow-hidden shadow-lg bg-gray-800 text-white hover:scale-105 hover:transition-transform transition-transform">
    <img class="w-full" :src="image" alt="Project Image">
    <div class="px-6 py-4">
      <div class="font-bold text-xl mb-2">{{ title }}</div>
      <p class="text-gray-400 text-base">
        {{ description }}
      </p>
    </div>
    <div class="px-6 py-4">
      <a :href="link" target="_blank" class="inline-block bg-green-500 text-white px-3 py-2 rounded font-semibold
        hover:bg-green-600 transition-colors
      ">
        View Project
      </a>
      &nbsp;
      <a :href="repo" target="_blank" class="inline-block bg-white text-green-500 px-3 py-2 rounded font-semibold
        hover:bg-gray-200 transition-colors
      ">
        Repo
      </a>
    </div>
  </div>
</template>

<script setup lang="ts">
  interface Props {
    title: string;
    description: string;
    image: string;
    link: string;
    repo: string;
  }

  defineProps<Props>();
</script>
