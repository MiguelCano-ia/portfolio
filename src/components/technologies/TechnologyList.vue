<template>
  <div>
    <h2 class="text-2xl text-green-500 mb-4 font-semibold text-center">{{ title }}</h2>
    <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-4 gap-6">
      <TechnologyCard v-for="(tech, index) in technologies" :key="index" :logo="tech.logo" :name="tech.name" />
    </div>
  </div>
</template>

<script setup lang="ts">
  import TechnologyCard from '@/components/technologies/TechnologyCard.vue'

  interface Props {
    title: string;
    technologies: { name: string; logo: string  }[];
  }

  defineProps<Props>();
</script>