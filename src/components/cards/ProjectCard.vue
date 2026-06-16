<script setup>
defineProps({
  project: Object
})
</script>

<template>
  <div class="project-card">

    <h3>
      {{ project.name }}
    </h3>

    <p>
      {{ project.description }}
    </p>

    <div class="tags">

      <span
        v-for="tech in project.tech"
        :key="tech"
      >
        {{ tech }}
      </span>

    </div>

    <a
      :href="project.github"
      target="_blank"
    >
      Ver repositorio
    </a>

  </div>
</template>

<style scoped>
.project-card {
  background: var(--bg-secondary);

  border: 1px solid var(--border);

  color: var(--text-primary);

  transition: .3s ease;
}

.project-card:hover {
  transform: translateY(-6px);

  border-color: var(--accent);
}
</style>