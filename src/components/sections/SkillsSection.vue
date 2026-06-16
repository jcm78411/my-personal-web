<script setup>
import SkillCard from '../cards/SkillCard.vue'
import { skills } from '../data/skills'
</script>

<template>
  <section
    id="skills"
    class="skills-section"
  >

    <div class="container">

      <h2>Habilidades Técnicas</h2>

      <div class="skills-grid">

        <SkillCard
          v-for="group in skills"
          :key="group.category"
          :skill-group="group"
        />

      </div>

    </div>

  </section>
</template>

<style scoped>

.skills-section {
  padding: 5rem 2rem;
}

.container {
  /* max-width: 1200px; */
  margin: 0 auto;
}

.skills-grid {
  display: grid;
  grid-template-columns:
    repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}

h2 {
  text-align: center;
  margin-bottom: 3rem;
}

</style>