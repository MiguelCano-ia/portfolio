<template>
  <div class="bg-gray-900 text-white p-6 rounded-lg shadow-lg mt-6">
    <h3 class="text-2xl font-bold mb-4 text-gray-300">Experiences & Studies</h3>
    <ul>
      <li v-for="(item, index) in experiences" :key="index" class="mb-2">
        <strong>{{ item.title }}</strong> - {{ item.description }}
      </li>
    </ul>
  </div>
</template>

<script setup lang="ts">
  interface Props {
    experiences: {
      title: string;
      description: string;
    }[];
  }

  defineProps<Props>();
</script>