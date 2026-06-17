<script setup>
import ExperienceCard from '../cards/ExperienceCard.vue'
import { experiences } from '../data/experience'
</script>

<template>
  <section id="experience" class="experience-section">
    <section class="py-16 px-4">
      <h1 class='font-semibold text-gray-900 text-3xl sm:text-4xl text-center mx-auto'>Dónde he trabajado...</h1>
      <p class='text-sm/relaxed text-gray-600 text-center mt-2 max-w-xl mx-auto'>Hear what our users say about us. We're
        always looking for ways to improve. If you have a positive experience with us, leave a review.</p>
      <div class="relative max-w-6xl mx-auto grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 px-4 md:px-0 pt-16">
        <div class='bg-gray-800 rounded-lg p-6 transform transition hover:-translate-y-1'>
          <p class='font-medium text-sm text-white mb-6'>Product Designer</p>
          <p class='text-sm text-gray-200 mb-4.5'>"This platform transformed our team collaboration. The interface and
            features make design work seamless."</p>
          <p class='text-xs text-gray-300'>- Sarah Chen</p>
        </div>
        <div class='bg-gray-800 rounded-lg p-6 transform transition hover:-translate-y-1'>
          <p class='font-medium text-sm text-white mb-6'>Software Engineer</p>
          <p class='text-sm text-gray-200 mb-4.5'>"Best investment for our workflow. The integration capabilities and
            optimization tools are outstanding."</p>
          <p class='text-xs text-gray-300'>- Marcus Johnson</p>
        </div>
        <div class='bg-gray-800 rounded-lg p-6 transform transition hover:-translate-y-1'>
          <p class='font-medium text-sm text-white mb-6'>Marketing Manager</p>
          <p class='text-sm text-gray-200 mb-4.5'>"Our campaign efficiency increased by 40%. The analytics dashboard
            provides insights we never had before."</p>
          <p class='text-xs text-gray-300'>- Emily Rodriguez</p>
        </div>
        <div class='bg-gray-800 rounded-lg p-6 transform transition hover:-translate-y-1'>
          <p class='font-medium text-sm text-white mb-6'>Startup Founder</p>
          <p class='text-sm text-gray-200 mb-4.5'>"As a small team, we needed something reliable and scalable. This
            exceeded our expectations and grew with us from day one."</p>
          <p class='text-xs text-gray-300'>- David Park</p>
        </div>
        <div class='bg-gray-800 rounded-lg p-6 transform transition hover:-translate-y-1'>
          <p class='font-medium text-sm text-white mb-6'>Content Creator</p>
          <p class='text-sm text-gray-200 mb-4.5'>"The automation features save me hours every week. I can finally focus
            on creating content rather than managing tedious tasks."</p>
          <p class='text-xs text-gray-300'>- Jessica Taylor</p>
        </div>
        <div class='bg-gray-800 rounded-lg p-6 transform transition hover:-translate-y-1'>
          <p class='font-medium text-sm text-white mb-6'>Sales Director</p>
          <p class='text-sm text-gray-200 mb-4.5'>"Our team closed 30% more deals this quarter thanks to the streamlined
            processes and real-time collaboration tools provided."</p>
          <p class='text-xs text-gray-300'>- Michael Anderson</p>
        </div>
      </div>
    </section>

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