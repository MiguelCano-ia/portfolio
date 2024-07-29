<template>
  <div class="bg-gray-900 p-6 md:p-12" id="about">
    <div class="max-w-[1320px] mx-auto">
      <ProfileCard
        name="More about me"
        description="I am Miguel Angel Cano Giraldo, a 20-year-old full-stack developer with a strong focus on frontend technologies. My passion lies in crafting intuitive and engaging user interfaces that provide seamless experiences. While I have a comprehensive understanding of backend development, I specialize in bringing design and functionality together on the frontend. My goal is to continuously improve my skills and stay updated with the latest trends in web development."
      />
      <ExperienceList
        :experiences="[
          { title: 'Cooding Bootcamp Technological University of Pereira', description: '+400 hours learning about FullStack development' },
          { title: 'Full Stack Diploma Technological University of Pereira and others institutes', description: '2023 Nov 12 - 2024 June 14' },
          { title: 'Computer and systems engineering at Technological University of Pereira', description: '2021 August - Currently studying' },
        ]"
      />
    </div>
  </div>
</template>

<script setup lang="ts">
import ProfileCard from '@/components/about/ProfileCard.vue'
import ExperienceList from '@/components/about/ExperienceList.vue'
</script>
