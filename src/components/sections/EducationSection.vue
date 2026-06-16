<script setup>
import EducationCard from '../cards/EducationCard.vue'
import { educationList } from '../data/education'
</script>

<template>
  <section
    id="education"
    class="education-section"
  >

    <div class="container">

      <h2>Formación Académica</h2>

      <div class="education-grid">

        <EducationCard
          v-for="item in educationList"
          :key="item.degree"
          :education="item"
        />

      </div>

    </div>

  </section>
</template>

<style scoped>

.education-section {
  padding: 5rem 2rem;
}

.container {
  /* max-width: 1200px; */
  margin: 0 auto;
}

.education-grid {
  display: grid;
  gap: 2rem;
}

h2 {
  text-align: center;
  margin-bottom: 3rem;
}

</style>