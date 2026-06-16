<script setup>
import ProjectCard from '../cards/ProjectCard.vue'
import { projects } from '../data/projects'
</script>

<template>
  <section id="projects">

    <h2>Proyectos</h2>

    <ProjectCard
      v-for="project in projects"
      :key="project.name"
      :project="project"
    />

  </section>
</template>