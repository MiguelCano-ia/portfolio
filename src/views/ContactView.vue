<template>
  <div class="p-6 flex flex-col items-center" id="contact">
    <h1 class="text-3xl text-gray-300 font-semibold mb-5">Contact Me</h1>
    <div class="flex space-x-4 gap-10 mb-10">
      <a href="https://github.com/MiguelCano-ia" class="text-white" target="_blank">
        <img :src="GitHubIcon" alt="GitHub" class="w-16 h-16"/>
      </a>
      <a href="mailto:m.cano1@utp.edu.co" class="text-white" target="_blank">
        <img :src="GmailIcon" alt="Gmail" class="w-16 h-16"/>
      </a>
      <a href="https://www.linkedin.com/in/miguel-angel-cano-giraldo-32a1ba253/" class="text-white" target="_blank">
        <img :src="LinkedInIcon" alt="LinkedIn" class="w-16 h-16"/>
      </a>
    </div>
  </div>

</template>

<script setup lang="ts">
  import GitHubIcon from '@/assets/icons/github.svg'
  import GmailIcon from '@/assets/icons/gmail.svg'
  import LinkedInIcon from '@/assets/icons/linkedin.svg'
</script>