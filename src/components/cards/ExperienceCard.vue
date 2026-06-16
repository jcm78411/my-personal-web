<script setup>
defineProps({
  experience: {
    type: Object,
    required: true
  }
})
</script>

<template>
  <article class="experience-card">

    <div class="header">

      <h3>
        {{ experience.title }}
      </h3>

      <span class="period">
        {{ experience.period }}
      </span>

    </div>

    <p class="description">
      {{ experience.description }}
    </p>

    <ul class="achievements">

      <li
        v-for="achievement in experience.achievements"
        :key="achievement"
      >
        {{ achievement }}
      </li>

    </ul>

  </article>
</template>

<style scoped>

.experience-card {
  border-radius: 12px;
  padding: 1.5rem;
  box-shadow: 0 4px 12px rgba(0,0,0,.08);
  transition: transform .2s ease;
  background: var(--bg-secondary);

  border: 1px solid var(--border);

  color: var(--text-primary);
}

.experience-card:hover {
  transform: translateY(-4px);
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: start;
  gap: 1rem;
  margin-bottom: 1rem;
}

h3 {
  margin: 0;
}

.period {
  font-size: .9rem;
  color: #666;
  white-space: nowrap;
}

.description {
  margin-bottom: 1rem;
  line-height: 1.6;
}

.achievements {
  padding-left: 1.2rem;
}

.achievements li {
  margin-bottom: .5rem;
}

/* @media (max-width: 768px) {
  .header {
    flex-direction: column;
  }
} */

</style>