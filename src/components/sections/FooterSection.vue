<template>
  <footer class="footer">

    <div class="container">

      <p>
        © {{ currentYear }} Juan Luis Cueto Morelo
      </p>

      <div class="links">

        <a
          href="https://github.com/jcm78411"
          target="_blank"
        >
          GitHub
        </a>

        <a
          href="https://linkedin.com/in/TU_USUARIO"
          target="_blank"
        >
          LinkedIn
        </a>

      </div>

    </div>

  </footer>
</template>

<script setup>
const currentYear = new Date().getFullYear()
</script>

<style scoped>
.footer {
  width: 100%;
  padding: 2rem;
  background: var(--bg-secondary);
  color: var(--text-primary);

  border-top: 1px solid var(--border);
}

.container {
  max-width: 30%;
  margin: 0 auto;

  display: flex;
  justify-content: space-between;
  align-items: center;
  place-items: center;
}

.links {
  display: flex;
  gap: 1rem;
}

a {
  color: white;
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

@media (max-width: 768px) {
  .container {
    flex-direction: column;
    gap: 1rem;
  }
}
</style>