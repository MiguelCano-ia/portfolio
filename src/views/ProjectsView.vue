<template>
  <div class="bg-gray-900 p-6 flex flex-col justify-center items-center" id="projects">
    <h1 class="text-4xl text-gray-300 font-semibold mb-8">Projects</h1>
    <div class="grid md:grid-cols-3 gap-20 mb-10">
      <ProjectCard
        title="Memorama Game with pure CSS"
        description="Exploring the full potential of css, team building this challenging game."
        :image=MemoramaImage
        link="https://funny-salmiakki-6d360d.netlify.app"
      />
      <ProjectCard
        title="Christmas Memorama"
        description="Another memory game with pure css, but with Christmas theme and more complexity."
        :image=ChritsmasMemorama
        link="https://amazing-dieffenbachia-f76a6c.netlify.app"
      />
      <ProjectCard
        title="News App"
        description="An advanced news app created in team with react and other tools, also using tailwind for styling and dark mode. "
        :image=NewsApp
        link="https://bootcamp-news.netlify.app/"
      />
      <ProjectCard
        title="Indecision App"
        description="Basic indecision app to learn the fundamentals of Vue, you need to use the question mark at the end of the message for interact with the API."
        :image=IndecisionApp
        link="https://visionary-semifreddo-4074b1.netlify.app"
      />
      <ProjectCard
        title="Cinema App"
        description="A movie app where fundamental concepts of reacting and filtering were reinforced."
        :image=CinemaApp
        link="https://cinema-app-omega.vercel.app/"
      />

    </div>
  </div>
</template>

<script setup lang="ts">
  import ProjectCard from '@/components/projects/ProjectCard.vue'
  import MemoramaImage from '../assets/memora.jpg'
  import IndecisionApp from '../assets/indecision.jpg'
  import NewsApp from '../assets/newsapp.jpg'
  import CinemaApp from '../assets/cinemapp.jpg'
  import ChritsmasMemorama from '../assets/memora2.jpg'
</script>