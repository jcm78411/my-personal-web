<script setup>
const currentYear = new Date().getFullYear();
</script>

<template>
  <footer class="footer">
    <footer
      class="flex flex-col items-center justify-center w-full py-20 text-white/70"
    >
      <img
        src="../icons/image.svg"
        alt="Logo"
        class="w-20 h-20"
        width="90"
        height="90"
      />
      <p class="mt-4 text-center">
        jcm78411 © {{ `${currentYear}` }} · Juan Luis Cueto Morelo.
      </p>
      <div class="flex items-center gap-4 mt-5">
        <a
          href="https://www.linkedin.com/in/juan-luis-cueto-morelo-bb72a9413/"
          class="hover:-translate-y-0.5 transition-all duration-300"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="26"
            height="26"
            viewBox="0 0 24 24"
          >
            <path
              fill="#cccccc"
              d="M20.47 2H3.53a1.45 1.45 0 0 0-1.47 1.43v17.14A1.45 1.45 0 0 0 3.53 22h16.94a1.45 1.45 0 0 0 1.47-1.43V3.43A1.45 1.45 0 0 0 20.47 2M8.09 18.74h-3v-9h3ZM6.59 8.48a1.56 1.56 0 1 1 0-3.12a1.57 1.57 0 1 1 0 3.12m12.32 10.26h-3v-4.83c0-1.21-.43-2-1.52-2A1.65 1.65 0 0 0 12.85 13a2 2 0 0 0-.1.73v5h-3v-9h3V11a3 3 0 0 1 2.71-1.5c2 0 3.45 1.29 3.45 4.06Z"
            />
          </svg>
        </a>

        <a
          href="https://github.com/jcm78411"
          class="hover:-translate-y-0.5 transition-all duration-300"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="26"
            height="26"
            viewBox="0 0 64 64"
          >
            <path
              fill="#cccccc"
              d="M32 0C14 0 0 14 0 32c0 21 19 30 22 30c2 0 2-1 2-2v-5c-7 2-10-2-11-5c0 0 0-1-2-3c-1-1-5-3-1-3c3 0 5 4 5 4c3 4 7 3 9 2c0-2 2-4 2-4c-8-1-14-4-14-15q0-6 3-9s-2-4 0-9c0 0 5 0 9 4c3-2 13-2 16 0c4-4 9-4 9-4c2 7 0 9 0 9q3 3 3 9c0 11-7 14-14 15c1 1 2 3 2 6v8c0 1 0 2 2 2c3 0 22-9 22-30C64 14 50 0 32 0"
            />
          </svg>
        </a>

        <a
          href="https://github.com/Jcuetomorelo37"
          class="hover:-translate-y-0.5 transition-all duration-300"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="26"
            height="26"
            viewBox="0 0 64 64"
          >
            <path
              fill="#cccccc"
              d="M32 0C14 0 0 14 0 32c0 21 19 30 22 30c2 0 2-1 2-2v-5c-7 2-10-2-11-5c0 0 0-1-2-3c-1-1-5-3-1-3c3 0 5 4 5 4c3 4 7 3 9 2c0-2 2-4 2-4c-8-1-14-4-14-15q0-6 3-9s-2-4 0-9c0 0 5 0 9 4c3-2 13-2 16 0c4-4 9-4 9-4c2 7 0 9 0 9q3 3 3 9c0 11-7 14-14 15c1 1 2 3 2 6v8c0 1 0 2 2 2c3 0 22-9 22-30C64 14 50 0 32 0"
            />
          </svg>
        </a>

        <a
          href="https://orcid.org/0009-0000-3190-5812"
          class="hover:-translate-y-0.5 transition-all duration-300"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="26"
            height="26"
            viewBox="0 0 32 32"
          >
            <path
              fill="#999999"
              d="M16 0C7.161 0 0 7.161 0 16s7.161 16 16 16s16-7.161 16-16S24.839 0 16 0M9.823 5.839c.704 0 1.265.573 1.265 1.26s-.561 1.265-1.265 1.265a1.27 1.27 0 0 1-1.26-1.265c0-.697.563-1.26 1.26-1.26m-.959 4.046h1.923v13.391H8.864zm4.751 0h5.197c4.948 0 7.125 3.541 7.125 6.703c0 3.439-2.687 6.699-7.099 6.699h-5.224zm1.921 1.74v9.927h3.063c4.365 0 5.365-3.312 5.365-4.964c0-2.687-1.713-4.963-5.464-4.963z"
            />
          </svg>
        </a>
      </div>
    </footer>
  </footer>
</template>

<style scoped>
.footer {
  width: 100%;
  padding: 1rem;
  color: var(--text-primary);

  border-top: 1px solid var(--border);
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
</style>
