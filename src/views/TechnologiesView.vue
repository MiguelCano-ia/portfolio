<template>
  <div class="bg-gray-900 p-6" id="technologies">
    <h1 class="text-4xl text-center mb-8 text-gray-300 font-semibold">Technologies</h1>
    <div class="flex flex-col mb-10">
      <div class="max-w-5xl mx-auto">
        <TechnologyList
          title="Frontend"
          :technologies="frontendTechnologies"
        />
        <TechnologyList
          title="Backend"
          :technologies="backendTechnologies"
        />
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
  import TechnologyList from '@/components/technologies/TechnologyList.vue'

  import JavaScriptLogo from '../assets/icons/javascript.svg'
  import TypeScriptLogo from '../assets/icons/typescript.svg'
  import VueJsLogo from '../assets/icons/vuejs.svg'
  import ReactLogo from '../assets/icons/react.svg'
  import NextLogo from '../assets/icons/nextjs.svg'

  import NodeLogo from '../assets/icons/nodejs.svg'
  import ExpressLogo from '../assets/icons/express.svg'
  import PostgresLogo from '../assets/icons/postgres.svg'
  import DockerLogo from '../assets/icons/docker.svg'


  const frontendTechnologies = [
    { name: 'JavaScript', logo: JavaScriptLogo },
    { name: 'TypeScript', logo: TypeScriptLogo },
    { name: 'Vue', logo: VueJsLogo },
    { name: 'React', logo: ReactLogo },
    { name: 'Next', logo: NextLogo },
  ]

  const backendTechnologies = [
    { name: 'Node', logo: NodeLogo },
    { name: 'Express', logo: ExpressLogo },
    { name: 'Postgres', logo: PostgresLogo },
    { name: 'Docker', logo: DockerLogo },
  ]
</script>