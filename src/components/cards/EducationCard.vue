<script setup>
defineProps({
  education: {
    type: Object,
    required: true
  }
})
</script>

<template>
  <article class="education-card">

    <h3>
      {{ education.degree }}
    </h3>

    <h4>
      {{ education.institution }}
    </h4>

    <span class="period">
      {{ education.period }}
    </span>

    <p>
      {{ education.description }}
    </p>

  </article>
</template>

<style scoped>

.education-card {
  background: var(--bg-secondary);

  border: 1px solid var(--border);

  color: var(--text-primary);
  padding: 1.5rem;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0,0,0,.08);
}

.period {
  display: block;
  margin: .75rem 0;
  color: #666;
}

h3,
h4 {
  margin: 0;
}

h4 {
  margin-top: .5rem;
  color: #42b883;
}

</style>