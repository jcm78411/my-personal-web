<template>
  <section id="about">
    <div id="about-head">
      <h3>Hola... Soy Juan Cueto...</h3>
      <h1 class="text-5xl font-semibold mx-auto">Sobre mí</h1>

      <p class="text-2xl text-slate-500 mt-2 w-full mx-auto">
        Ingeniero de Sistemas con enfoque en proyectos tecnológicos e
        investigación científica.
      </p>
    </div>

    <div
      class="w-full flex flex-col md:flex-row items-center justify-center gap-8 px-4 md:px-0 py-10"
    >
      <div id="description" class="w-2/3">
        <p class="text-base cursor-default text-slate-500 mt-2 w-full">
          Soy Ingeniero de Sistemas, egresado de la Universidad de Córdoba
          (Colombia), tengo conocimientos básicos e intermedios en programación
          en Python, desarrollo web front-end con HTML y JavaScript y back-end
          con Node.js.
        </p>
        <br />
        <p class="text-base cursor-default text-slate-500 mt-2 w-full">
          En cuanto al desarrollo, he trabajado con frameworks como Vue.js y
          Electron.js, así como con manejo de SQL y modelado de bases de datos.
        </p>
        <br />
        <p class="text-base cursor-default text-slate-500 mt-2 w-full">
          He participado en el desarrollo de proyectos académicos y sociales
          enfocados en temas como gestión de inventarios, monitoreo climático
          con IA, gestión de hardware y control de acceso de personal.
        </p>
        <br />
        <p class="text-base cursor-default text-slate-500 mt-2 w-full">
          Por otra parte, tengo interés en proyectos de IoT, Machine Learning e
          Inteligencia Artificial; y para demostrarlo, cuento con experiencia en
          divulgación científica, incluyendo artículos publicados en revistas
          indexadas y otros.
        </p>
        <br />
        <div class="cursor-default">
          <div
            class="group bg-white dark:bg-slate-800 rounded-xl shadow-md overflow-hidden border border-transparent hover:border-indigo-200 transform transition duration-300 hover:scale-105 hover:shadow-2xl p-5"
          >
            <div class="flex items-start gap-4">
              <div
                class="w-12 h-12 flex items-center justify-center bg-indigo-50 rounded-full text-indigo-600 text-lg transform transition duration-500 group-hover:rotate-12"
                aria-hidden="true"
              >
                💡
              </div>
              <div class="flex-1">
                <h4
                  class="text-base font-medium text-slate-700 dark:text-slate-100"
                >
                  Orientado al aprendizaje continuo...
                </h4>
                <p
                  class="text-sm text-slate-500 dark:text-slate-400 italic mt-1"
                >
                  y a la contribución técnica, tecnológica y social.
                </p>
                <div class="mt-3 flex flex-wrap gap-2">
                  <span
                    class="text-xs bg-indigo-50 text-indigo-600 px-3 rounded-full font-medium"
                  >
                    Aprendizaje
                  </span>
                  <span
                    class="text-xs bg-slate-50 text-slate-600 px-3 rounded-full"
                  >
                    Colaboración
                  </span>
                  <span
                    class="text-xs bg-slate-50 text-slate-600 px-3 rounded-full"
                  >
                    Innovación
                  </span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div id="stacks" class="w-1/3">
        <div class="flex flex-col gap-10 mt-6">
          <div
            class="card-hover flex items-center gap-4 p-4"
            style="--border-color: #059669"
          >
            <div
              class="w-12 h-9 flex items-center justify-center bg-indigo-50 border border-indigo-200 rounded"
            >
              <img
                class="w-7 h-7"
                src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxMjgiIGhlaWdodD0iMTI4IiB2aWV3Qm94PSIwIDAgMjQgMjQiPjxwYXRoIGZpbGw9IiMwNTk2NjkiIGZpbGwtcnVsZT0iZXZlbm9kZCIgZD0iTTE0Ljg4NCAyLjg4NEwxMS43NjggNmwzLjExNiAzLjExNmwtMS43NjggMS43NjhsLTQtNEw4LjIzMiA2bC44ODQtLjg4NGw0LTR6bTggMi4yMzJsLTQtNGwtMS43NjggMS43NjhMMjAuMjMyIDZsLTMuMTE2IDMuMTE2bDEuNzY4IDEuNzY4bDQtNEwyMy43NjggNnptLTUuMzc2IDEwLjU1NWEzLjg1OCAzLjg1OCAwIDAgMSA0Ljk5MiAzLjY4N3YxLjMwOGwtLjg3NC4yNzZsLTkuNSAzbC0uMTgzLjA1OEgwdi0yLjVoMTEuNTU3bDguMzUtMi42MzdhMS4zNiAxLjM2IDAgMCAwLTEuNjY0LS44MDNsLTUuOTUzIDEuODMyYTIuNSAyLjUgMCAwIDEtLjcyLjEwOEg2Ljc1di0yLjVoMy43NXYtLjc0bC01LjY4NC0xLjIxN0ExLjkxNSAxLjkxNSAwIDAgMCAyLjUgMTcuNDE1di4zMzVIMHYtLjMzNWE0LjQxNSA0LjQxNSAwIDAgMSA1LjM0LTQuMzE3bDYuNjcyIDEuNDNsLjk4OC4yMTJ2Mi4zMTh6IiBjbGlwLXJ1bGU9ImV2ZW5vZGQiLz48L3N2Zz4="
                alt=""
              />
            </div>
            <div>
              <h3 class="text-base font-medium text-slate-600">
                Saber, compartir, inspirar a otros
              </h3>
              <p class="text-sm text-slate-500">
                Desarrollo de contenido educativo y divulgación científica.
              </p>
            </div>
          </div>

          <div
            class="card-hover flex items-center gap-4"
            style="--border-color: #0891b2"
          >
            <div
              class="w-12 h-9 flex items-center justify-center bg-indigo-50 border border-indigo-200 rounded"
            >
              <img
                class="w-7 h-7"
                src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxMjgiIGhlaWdodD0iMTI4IiB2aWV3Qm94PSIwIDAgMjQgMjQiPjxwYXRoIGZpbGw9Im5vbmUiIHN0cm9rZT0iIzAyODRjNyIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIiBzdHJva2Utd2lkdGg9IjIiIGQ9Ik0xMCA1YTIgMiAwIDEgMCA0IDBhMiAyIDAgMSAwLTQgME0zIDE5YTIgMiAwIDEgMCA0IDBhMiAyIDAgMSAwLTQgMG0xNCAwYTIgMiAwIDEgMCA0IDBhMiAyIDAgMSAwLTQgMG0tOC01YTMgMyAwIDEgMCA2IDBhMyAzIDAgMSAwLTYgMG0zLTd2NG0tNS4zIDYuOGwyLjgtMm03LjggMmwtMi44LTIiLz48L3N2Zz4="
                alt=""
              />
            </div>
            <div>
              <h3 class="text-base font-medium text-slate-600">
                Más tecnología, más soluciones
              </h3>
              <p class="text-sm text-slate-500">
                Desarrollo de proyectos tecnológicos con impacto social.
              </p>
            </div>
          </div>
          <div
            class="card-hover flex items-center gap-4 p-4"
            style="--border-color: #4f46e5"
          >
            <div
              class="w-12 h-9 flex items-center justify-center bg-indigo-50 border border-indigo-200 rounded"
            >
              <img
                class="w-7 h-7"
                src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxMjgiIGhlaWdodD0iMTI4IiB2aWV3Qm94PSIwIDAgMjQgMjQiPjxwYXRoIGZpbGw9IiM0ZjQ2ZTUiIGQ9Ik0yMC45NCAxMS42OWMxLjY0LTIgMi4zOC00LjA4IDEuNDUtNS42OXMtMy4wOC0yLTUuNjUtMS41OWEuNDkuNDkgMCAwIDEtLjU0LS4zMUMxNS4yNyAxLjY3IDEzLjg2IDAgMTIgMFM4LjczIDEuNjcgNy44IDQuMWEuNDkuNDkgMCAwIDEtLjU0LjMxQzQuNjkgNCAyLjU0IDQuMzkgMS42MSA2cy0uMTkgMy42NyAxLjQ1IDUuNjlhLjQ4LjQ4IDAgMCAxIDAgLjYyQzEuNDIgMTQuMzMuNjggMTYuMzkgMS42MSAxOGMuNyAxLjIyIDIuMTEgMS43NCAzLjg4IDEuNzRhMTEgMTEgMCAwIDAgMS43Ny0uMTVhLjQ5LjQ5IDAgMCAxIC41NC4zMWMuOTMgMi40MyAyLjM0IDQuMSA0LjIgNC4xczMuMjctMS42NyA0LjItNC4xYS40OS40OSAwIDAgMSAuNTQtLjMxYTExIDExIDAgMCAwIDEuNzcuMTVjMS43NyAwIDMuMTgtLjUyIDMuODgtMS43NGMuOTMtMS42MS4xOS0zLjY3LTEuNDUtNS42OWEuNDguNDggMCAwIDEgMC0uNjJNMy4zNCA3Yy4yNy0uNDcgMS0uNzUgMi4xOS0uNzVhOCA4IDAgMCAxIDEgLjA3YS41LjUgMCAwIDEgLjQ3LjU5Yy0uMTIuNTktLjIyIDEuMTktLjMgMS44MWEuNDUuNDUgMCAwIDEtLjE5LjMzYy0uNDkuMzgtMSAuNzctMS40MiAxLjE2YS40Ny40NyAwIDAgMS0uMzguMTJhLjUuNSAwIDAgMS0uMzUtLjE5QzMuMzMgOC43NiAzIDcuNiAzLjM0IDdtMy41NyAxMC40OGEuNDcuNDcgMCAwIDEtLjM0LjJjLTEuNzEuMjEtMi44OC0uMDctMy4yMy0uNjhzMC0xLjc2IDEtMy4xNGEuNS41IDAgMCAxIC4zNS0uMTlhLjQ3LjQ3IDAgMCAxIC4zOC4xMmMuNDUuMzkuOTMuNzggMS40MiAxLjE2YS40NS40NSAwIDAgMSAuMTkuMzNjLjA4LjYyLjE4IDEuMjIuMyAxLjgxYS40Ni40NiAwIDAgMS0uMDcuMzltMi44OC0xM0MxMC40NyAyLjg3IDExLjMgMiAxMiAyczEuNTMuODcgMi4yMSAyLjQ1YS41MS41MSAwIDAgMS0uMzEuNjhjLS41Ni4xOC0xLjE0LjQtMS43MS42NGEuNS41IDAgMCAxLS4zOCAwYy0uNTctLjI0LTEuMTUtLjQ2LTEuNzEtLjY1YS41LjUgMCAwIDEtLjMtLjI2YS41My41MyAwIDAgMS0uMDEtLjQxWm00LjQyIDE1LjFDMTMuNTMgMjEuMTMgMTIuNyAyMiAxMiAyMnMtMS41My0uODctMi4yMS0yLjQ1YS41MS41MSAwIDAgMSAuMzEtLjY4Yy41Ni0uMTggMS4xNC0uNCAxLjcxLS42NGEuNS41IDAgMCAxIC4zOCAwYy41Ny4yNCAxLjE1LjQ2IDEuNzEuNjRhLjUuNSAwIDAgMSAuMy4yN2EuNTMuNTMgMCAwIDEgLjAxLjQxWm0xLjIzLTUuODJhLjUxLjUxIDAgMCAxLS4yMi4zOWMtLjQ2LjMtMSAuNjEtMS40Ny45MXMtMSAuNTctMS41My44MmEuNDkuNDkgMCAwIDEtLjQ0IDBjLS41LS4yNS0xLS41Mi0xLjUzLS44MnMtMS0uNjEtMS40Ny0uOTFhLjUxLjUxIDAgMCAxLS4yMi0uMzljMC0uNTUtLjA2LTEuMTMtLjA2LTEuNzNzMC0xLjE4LjA2LTEuNzNhLjUxLjUxIDAgMCAxIC4yMi0uMzljLjQ2LS4zIDEtLjYxIDEuNDctLjkxczEtLjU3IDEuNTMtLjgyYS40OS40OSAwIDAgMSAuNDQgMGMuNS4yNSAxIC41MiAxLjUzLjgyczEgLjYxIDEuNDcuOTFhLjUxLjUxIDAgMCAxIC4yMi4zOWMwIC41NS4wNiAxLjEzLjA2IDEuNzNzLS4wMiAxLjE1LS4wNiAxLjdaTTIwLjY2IDE3Yy0uMzUuNi0xLjUyLjg5LTMuMjMuNjhhLjUuNSAwIDAgMS0uNDMtLjU5Yy4xMi0uNTkuMjItMS4xOS4zLTEuODFhLjQ1LjQ1IDAgMCAxIC4xOS0uMzNjLjQ5LS4zOCAxLS43NyAxLjQyLTEuMTZhLjQ3LjQ3IDAgMCAxIC4zOC0uMTJhLjUuNSAwIDAgMSAuMzUuMTlDMjAuNjcgMTUuMjQgMjEgMTYuNCAyMC42NiAxN20tMS02Ljg2YS41LjUgMCAwIDEtLjM1LjE5YS40Ny40NyAwIDAgMS0uMzgtLjEyYy0uNDUtLjM5LS45My0uNzgtMS40Mi0xLjE2YS40NS40NSAwIDAgMS0uMTktLjMzYy0uMDgtLjYyLS4xOC0xLjIyLS4zLTEuODFhLjUuNSAwIDAgMSAuNDMtLjU5YTggOCAwIDAgMSAxLS4wN2MxLjE0IDAgMS45Mi4yOCAyLjE5Ljc1cy4wMyAxLjc2LTEgMy4xNFoiLz48cGF0aCBmaWxsPSIjNGY0NmU1IiBkPSJNMTAuMDQgMTJhMS45NiAxLjkxIDAgMSAwIDMuOTIgMGExLjk2IDEuOTEgMCAxIDAtMy45MiAwIi8+PC9zdmc+"
                alt=""
              />
            </div>
            <div>
              <h3 class="text-base font-medium text-slate-600">
                Contribución científica y social
              </h3>
              <p class="text-sm text-slate-500">
                Participación en eventos tecnológicos y contribuciones
                académicas.
              </p>
            </div>
          </div>

          <div
            class="card-hover flex items-center gap-4"
            style="--border-color: #c026d3"
          >
            <div
              class="w-12 h-9 flex items-center justify-center bg-indigo-50 border border-indigo-200 rounded"
            >
              <img
                class="w-7 h-7"
                src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxMjgiIGhlaWdodD0iMTI4IiB2aWV3Qm94PSIwIDAgNTEyIDUxMiI+PHBhdGggZmlsbD0iI2MwMjZkMyIgZmlsbC1ydWxlPSJldmVub2RkIiBkPSJtODUuMzMzIDE2MC42MTdsMTI4LTc0bC4wNDMuMDI1TDI1NiA2MmwtNDIuNjY3LTI0LjY2Nkw0Mi42NjcgMTM2djE5Ny4zMzNMODUuMzMzIDM1OHptODcuNTgxIDIzLjcwMWwxMDQuNDE5LTYwLjM2N2wxMDQuNDMgNjAuMzczbC0xMDQuNDE5IDYwLjM2OHptLTIzLjU4MSAzNS42NTFWMzQ2LjA1TDI1NiA0MDcuNzE2di0xMjYuMDh6bTI1NiAxMjYuMDgxbC0xMDYuNjY3IDYxLjY2NlYyODEuNjQ5bDEwNi42NjctNjEuNjY3em0tMTI4LTI3MS4zODNMNDQ4IDE3My4zMzN2MTk3LjMzNGwtMTcwLjY2NyA5OC42NjdsLTE3MC42NjYtOTguNjY3VjE3My4zMzN6IiBjbGlwLXJ1bGU9ImV2ZW5vZGQiLz48L3N2Zz4="
                alt=""
              />
            </div>
            <div>
              <h3 class="text-base font-medium text-slate-600">
                Apoyo en desarrollo de proyectos
              </h3>
              <p class="text-sm text-slate-500">
                Apoyo y seguimiento en desarrollo de proyectos tecnológicos y
                académicos.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
section#about {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  align-content: center;
  justify-content: center;
  align-items: center;
  padding: 20px 0px 20px 0px;
  margin: 5px 0px 5px 0px;
  /* width: 100%; */
}

div#about-head {
  margin-bottom: 25px;
  padding-bottom: 25px;
  padding-left: 0px;
  margin-left: 0px;
  width: 75%;
}

.mt-3.flex.flex-wrap.gap-2 {
  margin: 10px;
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.text-xs.bg-slate-50.text-slate-600.px-3.rounded-full,
.text-xs.bg-indigo-50.text-indigo-600.px-3.rounded-full.font-medium {
  padding: 5px 10px 5px 10px;
  font-size: 15px;
}

.w-12.h-12.flex.items-center.justify-center.bg-indigo-50.rounded-full.text-indigo-600.text-lg.transform.transition.duration-500.group-hover\:rotate-12 {
  margin: 5% 0% 5% 2%;
  cursor: default;
}

.text-base.cursor-default.text-slate-500.mt-2.w-full,
.text-base.font-medium.text-slate-600 {
  color: rgb(206, 199, 199);
}

.w-full.flex.flex-col.md\:flex-row.items-center.justify-center.gap-8.px-4.md\:px-0.py-10 {
  width: 75%;
  margin: 0px 15px 0px 15px;
}

.group.bg-white.dark\:bg-slate-800.rounded-xl.shadow-md.overflow-hidden.border.border-transparent.hover\:border-indigo-200.transform.transition.duration-300.hover\:scale-105.hover\:shadow-2xl.p-5 {
  width: 70%;
  padding: 10px;
}

.card-hover {
  position: relative;
  overflow: hidden;
  padding: 1rem;
  border-radius: 12px;
  cursor: pointer;
  transition:
    transform 0.3s ease,
    background-color 0.3s ease,
    box-shadow 0.3s ease;
}

.card-hover:hover {
  transform: scale(1.03);
  background-color: rgba(248, 250, 252, 0.096);
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.08);
}

/* Barra superior animada */
.card-hover::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 0;
  height: 3px;
  background: var(--border-color, #8b5cf6);
  transition: width 0.5s ease;
}

/* Activar animación */
.card-hover:hover::before {
  width: 100%;
}
</style>
