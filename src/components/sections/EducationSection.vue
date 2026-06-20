<script setup>
import EducationCard from "../cards/EducationCard.vue";
import { educationList } from "../data/education";
</script>

<template>
  <section id="education" class="education-section">
    <div class="text-center">
      <h1 class="text-3xl md:text-4xl font-bold text-gray-100">
        Formación Académica
      </h1>
      <p class="text-sm md:text-base text-gray-500 mt-4">
        Instituciones en las que me he certificado como profesional
      </p>
      &nbsp;

      <div class="flex flex-wrap justify-center gap-5 mt-16 text-left">
        <div
          class="flex flex-col items-start border border-gray-200 p-5 rounded-lg"
        >
          <svg
            width="44"
            height="40"
            viewBox="0 0 44 40"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M33.172 5.469q2.555 0 4.547 1.547a7.4 7.4 0 0 1 2.695 4.007q.47 1.711.469 3.61 0 2.883-1.125 5.86a22.8 22.8 0 0 1-3.094 5.577 33 33 0 0 1-4.57 4.922A35 35 0 0 1 26.539 35l-3.398-3.398q5.296-4.243 7.218-6.563 1.946-2.32 2.016-4.617-2.86-.329-4.781-2.461-1.923-2.133-1.922-4.992 0-3.117 2.18-5.297 2.202-2.203 5.32-2.203m-20.625 0q2.555 0 4.547 1.547a7.4 7.4 0 0 1 2.695 4.007q.47 1.711.469 3.61 0 2.883-1.125 5.86a22.8 22.8 0 0 1-3.094 5.577 33 33 0 0 1-4.57 4.922A35 35 0 0 1 5.914 35l-3.398-3.398q5.296-4.243 7.218-6.563 1.946-2.32 2.016-4.617-2.86-.329-4.781-2.461-1.922-2.133-1.922-4.992 0-3.117 2.18-5.297 2.202-2.203 5.32-2.203"
              fill="#2563EB"
            />
          </svg>
          <div class="flex items-center justify-center mt-3 gap-1">
            <svg
              width="16"
              height="15"
              viewBox="0 0 16 15"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M7.524.464a.5.5 0 0 1 .952 0l1.432 4.41a.5.5 0 0 0 .476.345h4.637a.5.5 0 0 1 .294.904L11.563 8.85a.5.5 0 0 0-.181.559l1.433 4.41a.5.5 0 0 1-.77.559L8.294 11.65a.5.5 0 0 0-.588 0l-3.751 2.726a.5.5 0 0 1-.77-.56l1.433-4.41a.5.5 0 0 0-.181-.558L.685 6.123A.5.5 0 0 1 .98 5.22h4.637a.5.5 0 0 0 .476-.346z"
                fill="#FF532E"
              />
            </svg>
            <svg
              width="16"
              height="15"
              viewBox="0 0 16 15"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M7.524.464a.5.5 0 0 1 .952 0l1.432 4.41a.5.5 0 0 0 .476.345h4.637a.5.5 0 0 1 .294.904L11.563 8.85a.5.5 0 0 0-.181.559l1.433 4.41a.5.5 0 0 1-.77.559L8.294 11.65a.5.5 0 0 0-.588 0l-3.751 2.726a.5.5 0 0 1-.77-.56l1.433-4.41a.5.5 0 0 0-.181-.558L.685 6.123A.5.5 0 0 1 .98 5.22h4.637a.5.5 0 0 0 .476-.346z"
                fill="#FF532E"
              />
            </svg>
            <svg
              width="16"
              height="15"
              viewBox="0 0 16 15"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M7.524.464a.5.5 0 0 1 .952 0l1.432 4.41a.5.5 0 0 0 .476.345h4.637a.5.5 0 0 1 .294.904L11.563 8.85a.5.5 0 0 0-.181.559l1.433 4.41a.5.5 0 0 1-.77.559L8.294 11.65a.5.5 0 0 0-.588 0l-3.751 2.726a.5.5 0 0 1-.77-.56l1.433-4.41a.5.5 0 0 0-.181-.558L.685 6.123A.5.5 0 0 1 .98 5.22h4.637a.5.5 0 0 0 .476-.346z"
                fill="#FF532E"
              />
            </svg>
            <svg
              width="16"
              height="15"
              viewBox="0 0 16 15"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M7.524.464a.5.5 0 0 1 .952 0l1.432 4.41a.5.5 0 0 0 .476.345h4.637a.5.5 0 0 1 .294.904L11.563 8.85a.5.5 0 0 0-.181.559l1.433 4.41a.5.5 0 0 1-.77.559L8.294 11.65a.5.5 0 0 0-.588 0l-3.751 2.726a.5.5 0 0 1-.77-.56l1.433-4.41a.5.5 0 0 0-.181-.558L.685 6.123A.5.5 0 0 1 .98 5.22h4.637a.5.5 0 0 0 .476-.346z"
                fill="#FF532E"
              /></svg
            ><svg
              width="16"
              height="15"
              viewBox="0 0 16 15"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M7.524.464a.5.5 0 0 1 .952 0l1.432 4.41a.5.5 0 0 0 .476.345h4.637a.5.5 0 0 1 .294.904L11.563 8.85a.5.5 0 0 0-.181.559l1.433 4.41a.5.5 0 0 1-.77.559L8.294 11.65a.5.5 0 0 0-.588 0l-3.751 2.726a.5.5 0 0 1-.77-.56l1.433-4.41a.5.5 0 0 0-.181-.558L.685 6.123A.5.5 0 0 1 .98 5.22h4.637a.5.5 0 0 0 .476-.346z"
                fill="#FF532E"
              />
            </svg>
          </div>
          <p class="certific text-sm mt-3 text-gray-500">
            Ingeniería De Sistemas y Telecomunicaciones.
          </p>

          <p class="text-sm mt-3 text-gray-500">
            Con énfasis en Redes de internet, TIC, IoT, desarrollo de software,
            IA, Machine Learning y sistemas de información.
          </p>
          <div class="flex items-center gap-3 mt-4">
            <div
              class="hidden sm:grid sm:size-15 sm:shrink-0 sm:place-content-center sm:rounded-full sm:border-2 sm:border-indigo-500"
              aria-hidden="true"
            >
              <div class="flex items-center">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="30"
                  height="30"
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
              <h2 class="text-lg text-gray-900 font-medium">
                Universidad De Córdoba
              </h2>
              <p class="text-sm text-gray-500">
                Monteria - Colombia @ Sept. 2025
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.education-section {
  padding: 5rem 2rem;
  width: 100%;
}

.container {
  /* max-width: 1200px; */
  margin: 0 auto;
}

.education-grid {
  display: grid;
  gap: 2rem;
}

h2 {
  text-align: center;
  margin-bottom: 3rem;
}

.flex.flex-col.items-start.border.border-gray-200.p-5.rounded-lg {
  padding: 20px;
  background: hsl(0, 3%, 75%);
  width: 30%;

  transition:
    transform 0.5s ease-in-out,
    background-color 0.5s ease-in-out;
}

.flex.flex-col.items-start.border.border-gray-200.p-5.rounded-lg:hover {
  scale: 1.02;
  background: hsla(0, 0%, 100%, 0.842);
  transform: scale(1.02);
}

.flex.items-center.gap-3.mt-4 {
  padding: 5px;
}

h2.text-lg.text-gray-900.font-medium {
  margin: 0;
}

.certific.text-sm.mt-3.text-gray-500{
padding: 5px 2px 5px 2px;
}
</style>
