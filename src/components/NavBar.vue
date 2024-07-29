<template>
  <nav class="bg-gray-900 text-white p-4">
    <ul class="flex flex-col gap-3 sm:flex-row sm:space-x-4 p-2 text-xl justify-center ">
      <li class="hover:text-green-500 transition-colors"><router-link to="/#home">Home</router-link></li>
      <li class="hover:text-green-500 transition-colors"><router-link to="/#projects">Projects</router-link></li>
      <li class="hover:text-green-500 transition-colors"><router-link to="/#about">About Me</router-link></li>
      <li class="hover:text-green-500 transition-colors"><router-link to="/#technologies">Technologies</router-link></li>
      <li class="hover:text-green-500 transition-colors"><router-link to="/#contact">Contact Me</router-link></li>
    </ul>
  </nav>
</template>

<script setup lang="ts">
</script>