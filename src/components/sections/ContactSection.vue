<script setup>
import { ref } from "vue";

const form = ref({
  name: "",
  email: "",
  message: "",
});

const loading = ref(false);
const success = ref(false);
const error = ref("");

const submitForm = async () => {
  loading.value = true;
  success.value = false;
  error.value = "";

  try {
    const payload = new URLSearchParams({
      "form-name": "contact",
      name: form.value.name,
      email: form.value.email,
      message: form.value.message,
    });

    const response = await fetch("/", {
      method: "POST",
      headers: {
        "Content-Type": "application/x-www-form-urlencoded",
      },
      body: payload.toString(),
    });

    if (!response.ok) {
      throw new Error("No fue posible enviar el formulario.");
    }

    success.value = true;

    form.value = {
      name: "",
      email: "",
      message: "",
    };
  } catch (err) {
    error.value = err.message;
  } finally {
    loading.value = false;
  }
};
</script>

<template>
  <section id="contact" class="contact-section">
    <h1
      class="text-3xl font-semibold mx-auto flex md:text-4xl font-bold text-gray-100"
    >
      Contacto
    </h1>
    <div class="contact-container">
      <div class="contact-grid">
        <div class="contact-info">
          <h2 class="contact-title">Tienes algún interés en común?</h2>
          <p class="contact-description">
            El mundo avanza, los intereses varían... si tienes a alguien que
            necesite asesorias sobre proyectos de mi área de conocimiento,
            alguna vacante disponible, un proyecto para trabajar, o quizás solo
            alguna idea que compartir... solo enviame un mensaje, estaré
            encantado de atenderte
          </p>

          <dl class="contact-list">
            <div>
              <dd class="contact-item">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="20"
                  height="20"
                  viewBox="0 0 16 16"
                >
                  <path
                    fill="#7c3aed"
                    d="M13.601 2.326A7.85 7.85 0 0 0 7.994 0C3.627 0 .068 3.558.064 7.926c0 1.399.366 2.76 1.057 3.965L0 16l4.204-1.102a7.9 7.9 0 0 0 3.79.965h.004c4.368 0 7.926-3.558 7.93-7.93A7.9 7.9 0 0 0 13.6 2.326zM7.994 14.521a6.6 6.6 0 0 1-3.356-.92l-.24-.144l-2.494.654l.666-2.433l-.156-.251a6.56 6.56 0 0 1-1.007-3.505c0-3.626 2.957-6.584 6.591-6.584a6.56 6.56 0 0 1 4.66 1.931a6.56 6.56 0 0 1 1.928 4.66c-.004 3.639-2.961 6.592-6.592 6.592m3.615-4.934c-.197-.099-1.17-.578-1.353-.646c-.182-.065-.315-.099-.445.099c-.133.197-.513.646-.627.775c-.114.133-.232.148-.43.05c-.197-.1-.836-.308-1.592-.985c-.59-.525-.985-1.175-1.103-1.372c-.114-.198-.011-.304.088-.403c.087-.088.197-.232.296-.346c.1-.114.133-.198.198-.33c.065-.134.034-.248-.015-.347c-.05-.099-.445-1.076-.612-1.47c-.16-.389-.323-.335-.445-.34c-.114-.007-.247-.007-.38-.007a.73.73 0 0 0-.529.247c-.182.198-.691.677-.691 1.654s.71 1.916.81 2.049c.098.133 1.394 2.132 3.383 2.992c.47.205.84.326 1.129.418c.475.152.904.129 1.246.08c.38-.058 1.171-.48 1.338-.943c.164-.464.164-.86.114-.943c-.049-.084-.182-.133-.38-.232"
                  />
                </svg>
                <span class="contact-text">+57 316 961 1670</span>
              </dd>
            </div>

            <div>
              <dd class="contact-item">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                >
                  <path
                    fill="#7550b4"
                    fill-rule="evenodd"
                    d="m7.172 11.334l2.83 1.935l2.728-1.882l6.115 6.033q-.242.079-.512.08H1.667c-.22 0-.43-.043-.623-.12zM20 6.376v9.457c0 .247-.054.481-.15.692l-5.994-5.914zM0 6.429l6.042 4.132l-5.936 5.858A1.7 1.7 0 0 1 0 15.833zM18.333 2.5c.92 0 1.667.746 1.667 1.667v.586L9.998 11.648L0 4.81v-.643C0 3.247.746 2.5 1.667 2.5z"
                  />
                </svg>
                <span class="contact-text">jcm78411@gmail.com</span>
              </dd>
            </div>

            <div>
              <dd class="contact-item">
                <!-- <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="20"
                  height="20"
                  viewBox="0 0 16 16"
                >
                  <path
                    fill="#7c3aed"
                    d="M13.601 2.326A7.85 7.85 0 0 0 7.994 0C3.627 0 .068 3.558.064 7.926c0 1.399.366 2.76 1.057 3.965L0 16l4.204-1.102a7.9 7.9 0 0 0 3.79.965h.004c4.368 0 7.926-3.558 7.93-7.93A7.9 7.9 0 0 0 13.6 2.326zM7.994 14.521a6.6 6.6 0 0 1-3.356-.92l-.24-.144l-2.494.654l.666-2.433l-.156-.251a6.56 6.56 0 0 1-1.007-3.505c0-3.626 2.957-6.584 6.591-6.584a6.56 6.56 0 0 1 4.66 1.931a6.56 6.56 0 0 1 1.928 4.66c-.004 3.639-2.961 6.592-6.592 6.592m3.615-4.934c-.197-.099-1.17-.578-1.353-.646c-.182-.065-.315-.099-.445.099c-.133.197-.513.646-.627.775c-.114.133-.232.148-.43.05c-.197-.1-.836-.308-1.592-.985c-.59-.525-.985-1.175-1.103-1.372c-.114-.198-.011-.304.088-.403c.087-.088.197-.232.296-.346c.1-.114.133-.198.198-.33c.065-.134.034-.248-.015-.347c-.05-.099-.445-1.076-.612-1.47c-.16-.389-.323-.335-.445-.34c-.114-.007-.247-.007-.38-.007a.73.73 0 0 0-.529.247c-.182.198-.691.677-.691 1.654s.71 1.916.81 2.049c.098.133 1.394 2.132 3.383 2.992c.47.205.84.326 1.129.418c.475.152.904.129 1.246.08c.38-.058 1.171-.48 1.338-.943c.164-.464.164-.86.114-.943c-.049-.084-.182-.133-.38-.232"
                  />
                </svg> -->
                <span class="contact-text"></span>
                <p>
                  Tambien puedes darle un vistazo a mis perfiles en el pie de
                  página...
                </p>
              </dd>
            </div>
          </dl>
        </div>

        <form
          class="contact-form"
          name="contact"
          method="POST"
          data-netlify="true"
          @submit.prevent="submitForm"
        >
          <input type="hidden" name="form-name" value="contact" />
          <div class="form-group">
            <label class="form-label">Name</label>
            <input
              v-model="form.name"
              name="name"
              class="form-input"
              type="text"
              required
            />
          </div>

          <div class="form-group">
            <label class="form-label">Email</label>
            <input
              v-model="form.email"
              name="email"
              class="form-input"
              type="email"
              required
            />
          </div>

          <div class="form-group">
            <label class="form-label">Message</label>
            <textarea
              v-model="form.message"
              name="message"
              class="form-textarea"
              required
            ></textarea>
          </div>

          <button type="submit" class="submit-button" :disabled="loading">
            {{ loading ? "Enviando..." : "Enviar mensaje" }}
          </button>

          <p v-if="success" class="success-message">
            Tu mensaje ha sido enviado correctamente.
          </p>

          <p v-if="error" class="error-message">
            {{ error }}
          </p>
        </form>
      </div>
    </div>
  </section>
</template>

<style scoped>

.success-message {
  margin-top: 1rem;
  color: #16a34a;
  font-weight: 500;
}

.error-message {
  margin-top: 1rem;
  color: #dc2626;
  font-weight: 500;
}
/* ==========================
   Contenedor principal
========================== */
h1.text-3xl.font-semibold.mx-auto.flex.md\:text-4xl.font-bold.text-gray-100 {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  align-content: center;
  justify-content: center;
  align-items: center;
  padding-bottom: 10px;
}

.contact-section {
  width: 100%;
  padding: 4rem 1rem;
}

.contact-container {
  max-width: 75%;
  margin: 0 auto;
  padding: 2rem 1rem;
}

.contact-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2rem;
}

/* ==========================
   Información de contacto
========================== */

.contact-info {
  padding: 1rem 0;
}

.contact-title {
  margin: 0;
  font-size: 1.875rem;
  font-weight: 700;
  line-height: 1.2;
  color: #bbbbbb;
}

.contact-description {
  margin-top: 1rem;
  line-height: 1.7;
  color: #686c74;
}

.contact-list {
  margin-top: 1.5rem;
}

.contact-list > div:not(:last-child) {
  margin-bottom: 0.75rem;
}

.contact-item {
  display: grid;
  grid-template-columns: 24px 1fr;
  align-items: center;
  gap: 0.5rem;
  color: #374151;
}

.contact-icon {
  width: 20px;
  height: 20px;
}

.contact-item svg {
  color: #6366f1;
}

.contact-text {
  font-weight: 500;
}

/* ==========================
   Formulario
========================== */

.contact-form {
  display: flex;
  flex-direction: column;
  gap: 1rem;

  padding: 1.5rem;

  background-color: #f3f4f6;
  border: 1px solid #d1d5db;
  border-radius: 0.5rem;

  backdrop-filter: blur(12px);

  box-shadow:
    0 10px 25px rgba(0, 0, 0, 0.08),
    0 2px 8px rgba(0, 0, 0, 0.04);
}

.form-group {
  display: flex;
  flex-direction: column;
}

.form-label {
  display: block;
  margin-bottom: 0.25rem;

  font-size: 0.875rem;
  font-weight: 500;

  color: #111827;
}

.form-input,
.form-textarea {
  width: 100%;
  box-sizing: border-box;

  padding: 0.625rem 0.75rem;

  border: 1px solid #d1d5db;
  border-radius: 0.5rem;

  background-color: #ffffff;
  color: #374151;

  font-size: 1rem;

  transition:
    border-color 0.2s ease,
    box-shadow 0.2s ease;
}

.form-input:focus,
.form-textarea:focus {
  outline: none;
  border-color: #6366f1;
  box-shadow: 0 0 0 3px rgba(99, 102, 241, 0.15);
}

.form-textarea {
  resize: none;
  min-height: 120px;
}

/* ==========================
   Botón
========================== */

.submit-button {
  width: 100%;

  padding: 0.75rem 3rem;

  border: 1px solid #4f46e5;
  border-radius: 0.5rem;

  background-color: #4f46e5;
  color: white;

  font-size: 0.875rem;
  font-weight: 500;

  cursor: pointer;

  transition:
    background-color 0.3s ease,
    color 0.3s ease,
    border-color 0.3s ease;
}

.submit-button:hover {
  background-color: transparent;
  color: hsl(189, 100%, 26%);
}

/* ==========================
   Responsive
========================== */

@media (min-width: 640px) {
  .contact-container {
    padding-left: 1.5rem;
    padding-right: 1.5rem;
  }

  .contact-title {
    font-size: 2rem;
  }
}

@media (min-width: 768px) {
  .contact-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (min-width: 1024px) {
  .contact-container {
    padding-left: 2rem;
    padding-right: 2rem;
  }
}

/* ==========================
   MODO OSCURO (Vue Scoped)
========================== */

:deep(.dark) .contact-title {
  color: #ffffff;
}

:deep(.dark) .contact-description,
:deep(.dark) .contact-item {
  color: #e5e7eb;
}

:deep(.dark) .contact-item svg {
  color: #818cf8;
}

:deep(.dark) .contact-form {
  background-color: #1f2937;
  border-color: #4b5563;
}

:deep(.dark) .form-label {
  color: #ffffff;
}

:deep(.dark) .form-input,
:deep(.dark) .form-textarea {
  background-color: #111827;
  border-color: #4b5563;
  color: #ffffff;
}

:deep(.dark) .form-input::placeholder,
:deep(.dark) .form-textarea::placeholder {
  color: #9ca3af;
}

:deep(.dark) .form-input:focus,
:deep(.dark) .form-textarea:focus {
  border-color: #818cf8;
  box-shadow: 0 0 0 3px rgba(129, 140, 248, 0.2);
}

:deep(.dark) .submit-button {
  background-color: #4f46e5;
  border-color: #4f46e5;
}

:deep(.dark) .submit-button:hover {
  background-color: #4338ca;
  border-color: #4338ca;
  color: #ffffff;
}
</style>
