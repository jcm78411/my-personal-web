<template>
  <article
    class="border border-slate-800 rounded-xl p-6 bg-slate-900 hover:border-slate-700 transition-all"
  >
    <p class="text-xs text-slate-500 uppercase tracking-wider">
      Certificación
    </p>

    <h3 class="text-xl font-semibold text-slate-100 mt-2">
      {{ certification.title }}
    </h3>

    <p class="text-slate-400 mt-3">
      {{ certification.certificationName }}
    </p>

    <div class="mt-5 space-y-2">
      <p class="text-sm text-slate-500">
        <span class="font-medium text-slate-300">
          Entidad:
        </span>
        {{ certification.issuer }}
      </p>

      <p class="text-sm text-slate-500">
        <span class="font-medium text-slate-300">
          Fecha:
        </span>
        {{ certification.issueDate }}
      </p>
    </div>
  </article>
</template>

<script setup>
defineProps({
  certification: {
    type: Object,
    required: true,
  },
});
</script>

<style scoped>
.grid.grid-cols-1.md\:grid-cols-2.lg\:grid-cols-3.gap-6 {
    display: block;
}

article.border.border-slate-800.rounded-xl.p-6.bg-slate-900.hover\:border-slate-700.transition-all
 {
    padding: 20px;
    margin: 15px 10px 20px 10px;
}

span.inline-flex.px-3.py-1.rounded-full.text-xs.bg-slate-800.text-slate-300 {
    padding: 5px 10px 5px 10px;
}
</style>