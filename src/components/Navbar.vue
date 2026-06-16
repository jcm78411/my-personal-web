<script setup>
import { ref } from "vue";

const menuOpen = ref(false);

const links = [
  { label: "Sobre mí", href: "#about" },
  { label: "Habilidades", href: "#skills" },
  { label: "Proyectos", href: "#projects" },
  { label: "Experiencia", href: "#experience" },
  { label: "Educación", href: "#education" },
  { label: "Contacto", href: "#contact" },
];

const toggleMenu = () => {
  menuOpen.value = !menuOpen.value;
};

const closeMenu = () => {
  menuOpen.value = false;
};

const emit = defineEmits(["open-cv"]);
</script>

<template>
  <div class="text-sm text-white w-full">
    <!-- Barra superior -->

    <div
      class="text-center font-medium py-2 bg-gradient-to-r from-sky-500 to-cyan-400"
    >
      <p>Disponible para oportunidades laborales y proyectos de desarrollo</p>
    </div>

    <!-- Navbar -->

    <nav
      class="relative h-[70px] flex items-center justify-between px-6 md:px-16 lg:px-24 xl:px-32 py-4 transition-all shadow bg-slate-900 text-slate-100 border-b border-slate-700"
    >
      <!-- Logo -->

      <a href="#hero" class="flex items-center">
        <div class="flex flex-col leading-none">
          <span
            class="text-xl font-bold bg-gradient-to-r from-violet-500 via-[#9938CA] to-[#E0724A] bg-clip-text text-transparent"
          >
            Juan Luis
          </span>

          <span class="text-xs tracking-wider text-gray-500 uppercase">
            Cueto Morelo
          </span>
        </div>
      </a>

      <!-- Desktop Menu -->

      <ul class="hidden md:flex items-center space-x-8 md:pl-28">
        <li v-for="link in links" :key="link.href">
          <a :href="link.href" class="nav-link">
            {{ link.label }}
          </a>
        </li>
      </ul>

      <!-- Desktop Button -->

      <button
        id="btn-pimary"
        @click="emit('open-cv')"
        class="md:inline hidden bg-white hover:bg-gray-50 border border-gray-300 ml-20 px-9 py-2 rounded-full active:scale-95 transition-all"
      >
        Ver CV
      </button>

      <!-- Mobile Button -->

      <button
        aria-label="menu-btn"
        type="button"
        class="inline-block md:hidden active:scale-90 transition"
        @click="toggleMenu"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="30"
          height="30"
          viewBox="0 0 30 30"
        >
          <path
            d="M3 7a1 1 0 1 0 0 2h24a1 1 0 1 0 0-2zm0 7a1 1 0 1 0 0 2h24a1 1 0 1 0 0-2zm0 7a1 1 0 1 0 0 2h24a1 1 0 1 0 0-2z"
          />
        </svg>
      </button>

      <!-- Mobile Menu -->

      <div
        v-show="menuOpen"
        class="absolute top-[70px] left-0 w-full bg-white shadow-sm p-6 md:hidden"
      >
        <ul class="flex flex-col space-y-4 text-lg">
          <li v-for="link in links" :key="link.href">
            <a :href="link.href" class="text-sm" @click="closeMenu">
              {{ link.label }}
            </a>
          </li>
        </ul>

        <button
          @click="
            emit('open-cv');
            closeMenu();
          "
          class="bg-white text-gray-600 border border-gray-300 mt-6 text-sm hover:bg-gray-50 active:scale-95 transition-all w-40 h-11 rounded-full"
        >
          Ver CV
        </button>
      </div>
    </nav>
  </div>
</template>

<style scoped>
button#btn-pimary {
  background: var(--accent);
  color: var(--bg-primary);
  border-radius: 999px;
  transition: 0.3s;
}

#btn-primary:hover {
  background: var(--accent-hover);
}

#viewer {
  padding: 5px 10px 5px 10px;
}
.nav-link {
  position: relative;
  transition: color 0.3s ease;
  margin: 0px 5px 0px 5px;
  border-radius: 0px 7px 0px 7px;
}

.nav-link::after {
  content: "";
  position: absolute;

  left: 0;
  bottom: -4px;

  width: 0;
  height: 2px;

  background: #7c3aed;

  transition: width 0.3s ease;
}

.nav-link:hover {
  color: #7c3aed;
}

.nav-link:hover::after {
  width: 100%;
}

.text-center.font-medium.py-2.bg-gradient-to-r.from-sky-500.to-cyan-400 {
  margin-bottom: 10px;
}
</style>
