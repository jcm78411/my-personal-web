<script setup>
import SkillCard from "../cards/SkillCard.vue";
// import { skills } from "../data/skills";
import { skills } from "../data/archivos";
</script>

<template>
  <section id="skills" class="skills-section w-full">
    <div class="align-items-center justify-center w-full">
      <h1 class="text-3xl font-semibold mx-auto">Habilidades</h1>
      <p class="text-lg h-10 text-slate-500 mt-2 mx-auto">
        Entre los conocimientos que poseo y las tecnologías que he usado están:
      </p>
    </div>

    <div class="flex flex-wrap items-center justify-center gap-8 pt-12">
      <!-- ============================================================================================================================ -->

      <div class="flex flex-wrap gap-6">
        <div
          v-for="skill in skills"
          :key="skill.title"
          class="group w-72 h-44 [perspective:1000px]"
        >
          <div
            class="relative h-full w-full transition-all duration-700 [transform-style:preserve-3d] group-hover:[transform:rotateY(180deg)]"
          >
            <!-- Frente -->
            <div
              class="absolute inset-0 rounded-2xl p-6 text-white shadow-xl [backface-visibility:hidden]"
              :class="`bg-gradient-to-br ${skill.gradient}`"
            >
              <div class="flex h-full flex-col justify-center items-center">
                <span class="text-xs uppercase tracking-widest opacity-80">
                  Especialidad
                </span>

                <h3 class="mt-2 text-2xl font-bold text-center">
                  {{ skill.title }}
                </h3>
              </div>
            </div>

            <!-- Atrás -->
            <div
              class="absolute inset-0 rounded-2xl bg-slate-900 p-6 text-white shadow-xl [transform:rotateY(180deg)] [backface-visibility:hidden]"
            >
              <div
                class="flex h-full flex-col justify-center items-center gap-3"
              >
                <h4 class="text-lg font-semibold">Tecnologías</h4>

                <div class="flex flex-wrap rounded-full text-sm gap-2">
                  <span
                    v-for="tech in skill.techs"
                    :key="tech.name"
                    :class="tech.color"
                  >
                    {{ tech.name }}
                  </span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- ============================================================================================================================ -->
      <!-- ============================================================================================================================ -->
      <!-- ============================================================================================================================ -->
    </div>
  </section>
</template>

<style scoped>
.skills-section {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  align-content: center;
  justify-content: center;
  justify-items: center;
  align-items: center;
  padding: 3% 0% 4% 0%;
}

.align-items-center.justify-center.w-full {
  /* padding-left: 15%; */
  width: 75%;
  padding-bottom: 2rem;
}

.flex.flex-wrap.items-center.justify-center.gap-8.pt-12 {
    width: 75%;
}

/* .skills-grid {

  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  align-content: center;
  justify-content: center;
  justify-items: center;
  align-items: center;
} */

h2 {
  text-align: center;
  margin-bottom: 3rem;
  /* transition: scale 0.3s ease; */
}

.tech-badge {
  border-radius: 9999px;
  padding: 0.25rem 0.75rem;
  height: 1.75rem;
  min-width: 5rem;
  white-space: nowrap;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: default;
  transition:
    transform 300ms ease,
    box-shadow 300ms ease;
}

.tech-badge:hover {
  transform: translateY(-4px) scale(1.1);
  box-shadow: 0 10px 25px rgba(255, 255, 255, 0.15);
}
</style>
