<script setup>
import ExperienceCard from '../cards/ExperienceCard.vue'
import { experiences } from '../data/experience'
</script>

<template>
  <section
    id="experience"
    class="experience-section"
  >

    <div class="container">

      <h2>Experiencia</h2>

      <div class="experience-grid">

        <ExperienceCard
          v-for="experience in experiences"
          :key="experience.title"
          :experience="experience"
        />

      </div>

    </div>

  </section>
</template>

<style scoped>

.experience-section {
  padding: 5rem 2rem;
}

.container {
  /* max-width: 1200px; */
  margin: 0 auto;
}

h2 {
  text-align: center;
  margin-bottom: 3rem;
}

.experience-grid {
  display: grid;
  gap: 2rem;
}

</style>