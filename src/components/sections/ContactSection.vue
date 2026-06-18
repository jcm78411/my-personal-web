<template>
  <section class="px-4 py-16">
    <div
      class="max-w-6xl mx-auto flex flex-col md:flex-row items-center justify-center gap-12 md:gap-16"
    >
      <!-- Texto -->
      <div class="flex flex-col mt-10">
        <p
          class="text-sm font-medium text-zinc-500 uppercase mb-2 text-center md:text-left"
        >
          Get In Touch
        </p>

        <h1
          class="text-5xl font-bold leading-tight text-zinc-900 max-w-xs mb-4 text-center md:text-left"
        >
          Let's build something real.
        </h1>

        <p
          class="text-base leading-6 text-zinc-400 max-w-xs text-center md:text-left"
        >
          Let's turn your ideas into meaningful products that solve real
          problems and create real impact.
        </p>
      </div>

      <!-- Formulario -->
      <div class="w-full max-w-sm border border-zinc-300 rounded-2xl p-8">
        <h2 class="text-base font-medium text-zinc-800 mb-6">
          Send Message
        </h2>

        <form class="flex flex-col gap-4">
          <div class="flex flex-col gap-2">
            <label class="text-xs text-zinc-400">
              Name
            </label>

            <input
              type="text"
              placeholder="Enter your name"
              class="w-full bg-zinc-50 border border-zinc-300 rounded-lg px-4 py-3 text-sm text-zinc-800 placeholder-zinc-400 outline-none focus:border-zinc-500 transition-colors"
            />
          </div>

          <div class="flex flex-col gap-2">
            <label class="text-xs text-zinc-400">
              Email
            </label>

            <input
              type="email"
              placeholder="Enter your email"
              class="w-full bg-zinc-50 border border-zinc-300 rounded-lg px-4 py-3 text-sm text-zinc-800 placeholder-zinc-400 outline-none focus:border-zinc-500 transition-colors"
            />
          </div>

          <div class="flex flex-col gap-2">
            <label class="text-xs text-zinc-400">
              Message
            </label>

            <textarea
              rows="4"
              placeholder="Your message..."
              class="w-full bg-zinc-50 border border-zinc-300 rounded-lg px-4 py-3 text-sm text-zinc-800 placeholder-zinc-400 outline-none focus:border-zinc-500 transition-colors resize-none"
            ></textarea>
          </div>

          <button
            type="submit"
            class="bg-black hover:bg-zinc-800 text-white text-base py-3 rounded-lg transition-colors mt-1"
          >
            Send Message
          </button>
        </form>
      </div>
    </div>
  </section>
</template>

<style scoped>

</style>
