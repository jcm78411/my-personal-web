<script setup>

import CertificationCard from "../cards/CertificationCard.vue";
import PublicationCard from "../cards/PublicationCard.vue";

import {
  certifications,
} from "../data/certifications";

import {
  publications,
} from "../data/publications";
</script>

<template>
  <section id="experience" class="experience-section">
    <h1 class="text-5xl font-medium text-slate-200 mt-6">
      Donde he trabajado y colaborado...
    </h1>

    <article class="rounded-xl p-4 ring-3 ring-indigo-50">
      <div class="flex items-start sm:gap-8">
        <div
          class="hidden sm:grid sm:size-20 sm:shrink-0 sm:place-content-center sm:rounded-full sm:border-2 sm:border-indigo-500"
          aria-hidden="true"
        >
          <div class="flex items-center gap-1">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="57"
              height="57"
              viewBox="0 0 780 621"
            >
              <path
                fill="#4f46e5"
                d="m390 86l390 156l-390 155L99 281c-18 15-31 39-33 66h7c8 0 14 6 14 14v37c0 8-6 14-14 14h-5l19 194c1 8-5 15-13 15H39c-8 0-14-7-14-15l20-194h-5c-8 0-15-6-15-14v-37c0-8 7-14 15-14h11c2-29 15-54 33-72L0 242zm-11 339l11 4l11-4l214-86l16 177c1 12-7 17-18 12l-84-43c-11-6-29-5-39 1l-81 46c-10 6-28 6-38 0l-81-46c-10-6-28-7-38-1l-85 43c-11 6-19 0-18-12l16-177z"
              />
            </svg>
          </div>
        </div>

        <div>
          <strong
            class="rounded-sm border border-indigo-500 bg-indigo-500 px-3 py-1.5 text-xs font-medium text-white"
          >
            &nbsp; #1 &nbsp;
          </strong>

          <h3 class="mt-4 text-lg font-medium sm:text-xl">
            <a class="hover:underline">
              Docente - Instituto Educativo Simón Bolívar
            </a>
          </h3>

          <p class="mt-1 text-sm text-gray-700">
            Durante mi desempeño como docente, tuve a cargo planificación y
            ejecución de actividades académicas en las áreas de STEAM,
            emprendimiento, creatividad, innovación, análisis de datos e
            inteligencia artificial. Desarrollando estrategias de enseñanza y
            evaluación, supervisando proyectos de emprendimiento e innovación,
            fomentando habilidades de pensamiento lógico, resolución de
            problemas y manejo de datos, y brindando asesoría en la formación
            integral de los estudiantes para fortalecer competencias en ciencia,
            tecnología, ingeniería, arte y matemáticas.
          </p>
          <br />

          <div class="mt-4 sm:flex sm:items-center sm:gap-2">
            <div class="flex items-center gap-1 text-gray-500">
              <svg
                class="size-4"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"
                ></path>
              </svg>

              <p class="text-xs font-medium">Febrero de 2022 - Junio de 2025</p>
            </div>
          </div>
        </div>
      </div>
    </article>

    <article class="rounded-xl p-4 ring-3 ring-indigo-50">
      <div class="flex items-start sm:gap-8">
        <div
          class="hidden sm:grid sm:size-20 sm:shrink-0 sm:place-content-center sm:rounded-full sm:border-2 sm:border-indigo-500"
          aria-hidden="true"
        >
          <div class="flex items-center gap-1">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="65"
              height="65"
              viewBox="0 0 28 28"
            >
              <path
                fill="#4f46e5"
                d="m12.167 17.802l-.006-.014a8 8 0 0 1-.36-.094l-.009-.003A8 8 0 0 1 8.708 16a8 8 0 1 1 13.257-6.75c.039.413-.3.75-.715.75c-.414 0-.745-.337-.793-.749A6.5 6.5 0 1 0 11.496 16l.04.017q.3.123.616.217A2 2 0 0 1 16 17a2 2 0 0 1-3.833.802m-.986 1.272a9.5 9.5 0 0 1-4.53-3.054A3 3 0 0 0 4 19v.715C4 23.433 8.21 26 14 26s10-2.708 10-6.285V19a3 3 0 0 0-3-3h-3.645a3.5 3.5 0 0 1-6.174 3.074M19 10c0-1.512-.67-2.867-1.731-3.784a5 5 0 1 0-5.624 8.195A3.5 3.5 0 0 1 14 13.5a3.5 3.5 0 0 1 2.356.911A5 5 0 0 0 19 10"
              />
            </svg>
          </div>
        </div>

        <div>
          <strong
            class="rounded-sm border border-indigo-500 bg-indigo-500 px-3 py-1.5 text-xs font-medium text-white"
          >
            &nbsp; #2 &nbsp;
          </strong>

          <h3 class="mt-4 text-lg font-medium sm:text-xl">
            <a class="hover:underline">
              Auxiliar - Talento Tech Universidad Tecnológica de Bolívar
            </a>
          </h3>

          <p class="mt-1 text-sm text-gray-700">
            Aunque no se hace valer como experiencia certificada, durante este
            tiempo participé en actividades como supervicion de desarrollo de
            proyectos, verificación de objetivos, asesorías particulares a los
            alumnos y compartir material didáctico.
          </p>
          <br />

          <div class="mt-4 sm:flex sm:items-center sm:gap-2">
            <div class="flex items-center gap-1 text-gray-500">
              <svg
                class="size-4"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"
                ></path>
              </svg>

              <p class="text-xs font-medium">Junio de 2025 - Julio de 2025</p>
            </div>
          </div>
        </div>
      </div>
    </article>

    <div
    class="w-full py-24 px-6"
  >
    <div class="max-w-7xl mx-auto">

      <!-- CERTIFICACIONES -->

      <div>
        <h2
          class="text-4xl font-semibold text-slate-100"
        >
          Certificaciones
        </h2>

        <p
          class="text-slate-400 mt-3 mb-10"
        >
          Credenciales y formación profesional.
        </p>

        <div
          class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6"
        >
          <CertificationCard
            v-for="item in certifications"
            :key="item.id"
            :certification="item"
          />
        </div>
      </div>

      <!-- PUBLICACIONES -->

      <div class="mt-24">
        <h2
          class="text-4xl font-semibold text-slate-100"
        >
          Publicaciones
        </h2>

        <p
          class="text-slate-400 mt-3 mb-10"
        >
          Artículos científicos, libros y
          publicaciones académicas.
        </p>

        <div
          class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6"
        >
          <PublicationCard
            v-for="item in publications"
            :key="item.id"
            :publication="item"
          />
        </div>
      </div>

    </div>
    </div>
  </section>
</template>

<style scoped>
.experience-section {
  align-items: center;
  justify-content: center;
  justify-items: center;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  align-content: center;
  width: 100%;
  padding: 4% 7% 4% 7%;
}

article{
  width: 100%;
}

.container {
  /* max-width: 1200px; */
  margin: 0 auto;
}

h2 {
  text-align: center;
  margin-bottom: 3rem;
}

.experience-grid {
  display: grid;
  gap: 2rem;
}

.text-5xl.font-medium.text-slate-200.mt-6 {
  padding-bottom: 2rem;
}

h1.text-5xl.font-medium.text-slate-200.mt-6 {
  width: 75%;
}

article {
  transition:
    transform 0.5s ease-in-out,
    background-color 0.5s ease-in-out;
}

article:hover {
  background-color: rgba(79, 70, 229, 0.1);
  transform: scale(1.02);
}

.rounded-xl.p-4.ring-3.ring-indigo-50 {
  padding: 10px;
  margin-bottom: 20px;
}

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

.text-4xl.font-semibold.text-slate-100{
  margin-top: 25px;
}
</style>
