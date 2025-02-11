<template>
  <div class="bg-gray-900 p-6 flex flex-col justify-center items-center" id="projects">
    <h1 class="text-4xl text-gray-300 font-semibold mb-8">Projects</h1>
    <div class="grid md:grid-cols-3 gap-20 mb-10">
      <ProjectCard
        title="Tail News"
        description="An advanced news app created using an extarnal api (NewsApi), using backend as a service (firebase), also using tailwind for styling and dark mode and react with typescript for user interface "
        :image="TailNews"
        link="https://tail-news-rho.vercel.app/"
        repo="https://github.com/MiguelCano-ia/tail-news"
      />
      <ProjectCard
        title="World's Ranks"
        description="React app for exploring countries with advanced filters and search, using and external API."
        :image="WorldRank"
        link="https://world-ranks-livid-eight.vercel.app/"
        repo="https://github.com/MiguelCano-ia/world-ranks"
      />
      <ProjectCard
        title="Memorama Game with pure CSS"
        description="Exploring the full potential of css, team building this challenging game."
        :image="MemoramaImage"
        link="https://funny-salmiakki-6d360d.netlify.app"
        repo="https://github.com/MiguelCano-ia/memory-game"
      />
      <ProjectCard
        title="Christmas Memorama"
        description="Another memory game with pure css, but with Christmas theme and more complexity."
        :image="ChritsmasMemorama"
        link="https://amazing-dieffenbachia-f76a6c.netlify.app"
        repo="https://github.com/MiguelCano-ia/building-manger/tree/main/css"
      />
    </div>
  </div>
</template>

<script setup lang="ts">
import ProjectCard from '@/components/projects/ProjectCard.vue'
import MemoramaImage from '../assets/memora.jpg'
import TailNews from '../assets/tailnews.png'
import ChritsmasMemorama from '../assets/memora2.jpg'
import WorldRank from '../assets/worldranks.png'
</script>
