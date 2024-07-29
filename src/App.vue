<script setup lang="ts">
  import NavBar from '@/components/NavBar.vue'
  import HomeView from '@/views/HomeView.vue'
  import ProjectsView from '@/views/ProjectsView.vue'
  import AboutView from '@/views/AboutView.vue'
  import TechnologiesView from '@/views/TechnologiesView.vue'
  import ContactView from '@/views/ContactView.vue'
  import FooTer from '@/components/FooTer.vue'
  import BackTop from '@/components/BackTop.vue'
</script>

<template>
  <header>
    <NavBar />
  </header>
  <main class="bg-slate-900">
    <HomeView />
    <ProjectsView />
    <AboutView />
    <TechnologiesView />
    <ContactView />
    <BackTop />
  </main>
  <footer>
    <FooTer />
  </footer>
</template>

<style scoped>
</style>
