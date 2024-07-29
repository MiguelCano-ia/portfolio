<template>
  <button
    v-if="visible"
    @click="scrollToTop"
    class="fixed bottom-4 right-4 bg-green-500 text-white p-2 rounded-full shadow-lg hover:bg-green-700 transition-colors"
  >
    <svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 10l7-7m0 0l7 7m-7-7v18"></path>
    </svg>
  </button>
</template>

<script setup lang="ts">
  import { ref, onMounted, onUnmounted } from 'vue';

  // Composable logic
  const visible = ref(false);

  const toggleVisibility = () => {
    visible.value = window.scrollY > 200;
  };

  const scrollToTop = () => {
    window.scrollTo({
      top: 0,
      behavior: 'smooth',
    });
  };

  onMounted(() => {
    window.addEventListener('scroll', toggleVisibility);
  });

  onUnmounted(() => {
    window.removeEventListener('scroll', toggleVisibility);
  });
</script>
