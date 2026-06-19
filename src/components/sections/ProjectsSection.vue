<script setup>
import ProjectCard from "../cards/ProjectCard.vue";
import { projects } from "../data/projects";

import Networking from "../icons/Networking.vue";
import Schoolar from "../icons/Schoolar.vue";
import Plastics from "../icons/Plastics.vue";
import Chatbot from "../icons/Chatbot.vue";

const icons = {
  network: Networking,
  school: Schoolar,
  plastics: Plastics,
  chatbot: Chatbot,
};
</script>

<template>
  <section id="projects">
    <div class="w-full py-20 px-6 flex flex-col items-center">
      <div class="text-center mx-auto head-projects">
        <h1 class="text-4xl md:text-5xl font-medium text-slate-200 mt-6">
          Proyectos que he trabajado
        </h1>
        <p
          class="text-sm md:text-base text-slate-400 mt-3 max-w-[530px] mx-auto"
        >
          Algunos de los proyectos más relevantes en los que he trabajado y
          colaborado.
        </p>
      </div>

      <!--  Features Grid  -->
      <div class="eddd">
        <!-- ====================================================================================================================== -->
        <!-- ====================================================================================================================== -->
        <div
          class="w-full max-w-6xl mx-auto mt-16 grid gap-6 auto-rows-[220px] md:grid-cols-3 whitespace-pre-line"
        >
          <ProjectCard
            v-for="(project, index) in projects"
            :key="project.title"
            :title="project.title"
            :description="project.description"
            :button-text="project.buttonText"
            :link="project.link"
            :featured="index === 0"
            :class="index === 0 ? 'md:col-span-2 md:row-span-2' : ''"
          >
            <template #icon>
              <component :is="icons[project.icon]" />
            </template>
          </ProjectCard>
        </div>
        <!-- ====================================================================================================================== -->
        <!-- ====================================================================================================================== -->
      </div>
    </div>
  </section>
</template>

<style scoped>
section#projects {
  align-items: center;
  justify-content: center;
  justify-items: center;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  align-content: center;
  width: 100%;
  padding: 3% 0% 4% 0%;
}

.text-center.mx-auto.head-projects {
  padding-bottom: 2rem;
}

</style>
