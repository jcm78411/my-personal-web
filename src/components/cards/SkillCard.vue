<script setup>
defineProps({
  skillGroup: {
    type: Object,
    required: true,
  },
});
</script>

<template>
  <article class="skill-card">
    <h3>
      {{ skillGroup.category }}
    </h3>

    <div class="skills-container">
      <span v-for="skill in skillGroup.items" :key="skill" class="skill-badge">
        {{ skill }}
      </span>
    </div>
  </article>
</template>

<style scoped>
.skill-card {
  padding: 1.5rem;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
  background: var(--accent);
  color: var(--bg-primary);
}

.skills-container {
  display: flex;
  flex-wrap: wrap;
  gap: 0.75rem;
  margin-top: 1rem;
}

.skill-badge {
  padding: 0.4rem 0.8rem;
  border-radius: 999px;
  background: var(--accent);
  color: var(--bg-primary);
  color: white;
  font-size: 0.9rem;
}
</style>
