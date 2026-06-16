<!-- https://drive.google.com/file/d/1DL4I607BAAM2zIUL7XbJOEidWwA9WIrA/preview -->

<script setup>
defineProps({
  isOpen: {
    type: Boolean,
    default: false,
  },
});

const emit = defineEmits(["close"]);
</script>

<template>
  <div
    v-if="isOpen"
    class="fixed inset-0 z-50 flex items-center justify-center bg-slate-950/80 backdrop-blur-sm"
    @click.self="emit('close')"
  >
    <div
      class="bg-slate-800 text-slate-100 w-[95vw] h-[90vh] rounded-xl overflow-hidden shadow-2xl flex flex-col border border-slate-700"
    >
      <!-- Header -->

      <div
        class="flex justify-between items-center p-4 border-b border-slate-700"
      >
        <h2 class="font-semibold text-lg">Hoja de Vida</h2>

        <button
          @click="emit('close')"
          class="px-3 py-1 rounded-lg text-slate-300 hover:bg-slate-700 hover:text-white transition"
        >
          ✕
        </button>
      </div>

      <!-- PDF -->

      <iframe
        class="flex-1 w-full"
        src="https://drive.google.com/file/d/1DL4I607BAAM2zIUL7XbJOEidWwA9WIrA/preview"
      />

      <!-- Footer -->

      <div class="p-4 border-t border-slate-700 flex justify-end gap-3">
        <a
          style="padding: 10px; display: flex"
          href="https://drive.google.com/file/d/1DL4I607BAAM2zIUL7XbJOEidWwA9WIrA/view"
          target="_blank"
          class="px-4 py-2 border border-slate-600 text-slate-200 rounded-full hover:bg-slate-700 transition"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="20"
            height="20"
            viewBox="0 0 24 24"
          >
            <path
              fill="#059669"
              d="m16.9 20.5l-1.4-1.4l3.075-3.1H16v-2h6v6h-2v-2.6zm-11.4 1q-.425 0-.862-.262T4 20.625L1.5 16.25q-.2-.35-.2-.862t.2-.863L8 3.375q.2-.35.638-.613T9.5 2.5h5q.425 0 .863.263t.637.612l4.55 7.8q-.575-.15-1.187-.2t-1.213.05L14.35 4.5h-4.7L3.3 15.4l2.35 4.1h7.9q.275.575.638 1.075t.837.925zM7.25 17l-.725-1.275L11.1 7.75h1.8l2.525 4.4q-.425.325-.787.712t-.638.813L12 10.2L9.25 15h4.1q-.175.475-.262.975T13 17z"
            />
          </svg>
          &nbsp; Abrir en Drive
        </a>

        <a
          style="padding: 10px; display: flex"
          href="https://drive.google.com/uc?export=download&id=1DL4I607BAAM2zIUL7XbJOEidWwA9WIrA"
          class="px-4 py-2 rounded-full bg-sky-100 hover:bg-sky-200 text-slate-900 font-medium transition"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="20"
            height="20"
            viewBox="0 0 20 20"
          >
            <path
              fill="#059669"
              d="M15 7h-3V1H8v6H5l5 5zm4.338 6.532c-.21-.224-1.611-1.723-2.011-2.114A1.5 1.5 0 0 0 16.285 11h-1.757l3.064 2.994h-3.544a.27.27 0 0 0-.24.133L12.992 16H7.008l-.816-1.873a.28.28 0 0 0-.24-.133H2.408L5.471 11H3.715c-.397 0-.776.159-1.042.418c-.4.392-1.801 1.891-2.011 2.114c-.489.521-.758.936-.63 1.449l.561 3.074c.128.514.691.936 1.252.936h16.312c.561 0 1.124-.422 1.252-.936l.561-3.074c.126-.513-.142-.928-.632-1.449"
            />
          </svg>
          &nbsp; Descargar
        </a>
      </div>
    </div>
  </div>
</template>

<style scoped>
.flex.justify-between.items-center.p-4.border-b.border-slate-700 {
  padding: 5px 20px 5px 20px;
}

.p-4.border-t.border-slate-700.flex.justify-end.gap-3 {
  padding: 5px 20px 5px 20px;
}

</style>
