<script setup>
import { computed } from "vue";

const props = defineProps({
  title: String,
  description: String,
  buttonText: String,
  link: {
    type: String,
    default: "#",
  },
  featured: {
    type: Boolean,
    default: false,
  },
});

const links = computed(() => {
  if (!props.link) return [];
  return props.link.split("|").map((l) => l.trim());
});
</script>

<template>
  <div class="card-unit">
    <div
      class="group rounded-3xl border border-slate-800 bg-slate-900/50 p-6 hover:bg-slate-900 transition-all duration-300 h-full"
      :class="featured ? 'md:p-8' : ''"
    >
      <div
        class="size-13 flex items-center justify-center border border-slate-700 rounded-xl mb-6"
      >
        <slot name="icon" />
      </div>

      <h3
        class="font-semibold text-slate-100"
        :class="featured ? 'text-2xl' : 'text-lg'"
      >
        {{ title }}
      </h3>

      <p
        class="text-slate-400 mt-3"
        :class="featured ? 'text-base max-w-lg' : 'text-sm'"
      >
        {{ description }}
      </p>

      <!-- <a
      :href="link"
      class="mt-6 inline-flex items-center gap-2 text-sky-400 hover:text-sky-300"
    >
      {{ buttonText }}

      <svg
        class="transition-transform group-hover:translate-x-1"
        xmlns="http://www.w3.org/2000/svg"
        width="16"
        height="16"
        viewBox="0 0 24 24"
        fill="none"
        stroke="currentColor"
        stroke-width="1.5"
      >
        <path d="M5 12h14" />
        <path d="m12 5 7 7-7 7" />
      </svg>
    </a> -->
      <div class="mt-6 flex gap-4 flex-wrap">
        <a
          v-for="l in links"
          :key="l"
          :href="l"
          target="_blank"
          class="inline-flex items-center gap-2 text-sky-400 hover:text-sky-300"
        >
          {{ buttonText }}

          <svg
        class="transition-transform group-hover:translate-x-1"
        xmlns="http://www.w3.org/2000/svg"
        width="16"
        height="16"
        viewBox="0 0 24 24"
        fill="none"
        stroke="currentColor"
        stroke-width="1.5"
      >
        <path d="M5 12h14" />
        <path d="m12 5 7 7-7 7" />
      </svg>
        </a>
      </div>
    </div>
  </div>
</template>

<style scoped>
.group.rounded-3xl.border.border-slate-800.bg-slate-900\/50.p-6.hover\:bg-slate-900.transition-all.duration-300.h-full {
  padding: 20px;
}

.group.rounded-3xl.border.border-slate-800.bg-slate-900\/50.p-6.hover\:bg-slate-900.transition-all.duration-300.h-full.md\:p-8 {
  padding: 20px;
}
</style>
