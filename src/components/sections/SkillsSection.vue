<script setup>
import SkillCard from '../cards/SkillCard.vue'
import { skills } from '../data/skills'
</script>

<template>
  <section id="skills" class="skills-section">
    <h1 class="text-3xl font-semibold text-center mx-auto">Latest Blog</h1>
    <p class="text-sm text-slate-500 text-center mt-2 max-w-lg mx-auto">
      Stay ahead of the curve with fresh content on code, design, startups, and everything in between.
    </p>

    <div class="flex flex-wrap items-center justify-center gap-8 pt-12">
      <div class="max-w-72 w-full hover:-translate-y-0.5 transition duration-300">
        <img class="rounded-xl"
          src="https://images.unsplash.com/photo-1590650516494-0c8e4a4dd67e?w=1200&h=800&auto=format&fit=crop&q=60"
          alt="">
        <h3 class="text-base text-slate-900 font-medium mt-3">Color Psychology in UI: How to Choose the Right Palette
        </h3>
        <p class="text-xs text-indigo-600 font-medium mt-1">UI/UX design</p>
      </div>
      <div class="max-w-72 w-full hover:-translate-y-0.5 transition duration-300">
        <img class="rounded-xl"
          src="https://images.unsplash.com/photo-1714974528646-ea024a3db7a7?w=1200&h=800&auto=format&fit=crop&q=60"
          alt="">
        <h3 class="text-base text-slate-900 font-medium mt-3">Color Psychology in UI: How to Choose the Right Palette
        </h3>
        <p class="text-xs text-indigo-600 font-medium mt-1">UI/UX design</p>
      </div>
      <div class="max-w-72 w-full hover:-translate-y-0.5 transition duration-300">
        <img class="rounded-xl"
          src="https://images.unsplash.com/photo-1713947501966-34897f21162e?w=1200&h=800&auto=format&fit=crop&q=60"
          alt="">
        <h3 class="text-base text-slate-900 font-medium mt-3">Color Psychology in UI: How to Choose the Right Palette
        </h3>
        <p class="text-xs text-indigo-600 font-medium mt-1">UI/UX design</p>
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