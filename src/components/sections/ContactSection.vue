<template>
  <section id="contact">
<div class="flex items-center justify-center px-4 py-20">
    <div class="max-w-5xl w-full grid grid-cols-1 md:grid-cols-2 gap-12 lg:gap-20">

        <div class="flex flex-col items-start text-left">
            <div class="inline-flex items-center justify-center border border-zinc-200 bg-zinc-50 rounded-full px-4 py-1.5 text-sm text-zinc-800 mb-4">
                Contáctame
            </div>
            <h1 class="text-[40px] font-medium text-zinc-900 leading-tight mb-1.5">
                Tienes preguntas? Estoy aquí para ayudarte.
            </h1>
            <p class="text-sm text-zinc-600 max-w-[360px] mb-6 leading-relaxed">
                ¿Necesitas ayuda con componentes, configuración o personalización? Estamos aquí para apoyarte.
            </p>

            <div class="flex flex-col space-y-5">
                <div class="flex items-center gap-2">
                    <div class="size-9 rounded-full bg-zinc-100 flex items-center justify-center shrink-0">
                        <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="m18.333 5.836-7.492 4.772a1.67 1.67 0 0 1-1.674 0l-7.5-4.772" stroke="#71717b" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/><path d="M16.667 3.336H3.333c-.92 0-1.666.746-1.666 1.667v10c0 .92.746 1.666 1.666 1.666h13.334c.92 0 1.666-.746 1.666-1.666v-10c0-.92-.746-1.667-1.666-1.667" stroke="#71717b" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
                    </div>
                    <span class="text-sm text-zinc-600">hello@prebuiltUI.com</span>
                </div>

                <div class="flex items-center gap-2">
                    <div class="size-9 rounded-full bg-zinc-100 flex items-center justify-center shrink-0">
                        <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg"><g clip-path="url(#a)"><path d="M11.527 13.804a.83.83 0 0 0 1.01-.252l.296-.388a1.67 1.67 0 0 1 1.334-.667h2.5a1.667 1.667 0 0 1 1.666 1.667v2.5a1.667 1.667 0 0 1-1.666 1.667 15 15 0 0 1-15-15 1.667 1.667 0 0 1 1.666-1.667h2.5A1.667 1.667 0 0 1 7.5 3.331v2.5a1.67 1.67 0 0 1-.667 1.333l-.39.293A.83.83 0 0 0 6.2 8.484a11.67 11.67 0 0 0 5.327 5.32" stroke="#71717b" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></g><defs><clipPath id="a"><path fill="#fff" d="M0 0h20v20H0z"/></clipPath></defs></svg>
                    </div>
                    <span class="text-sm text-zinc-600">+91-9341555-010</span>
                </div>

                <div class="flex items-center gap-2">
                    <div class="size-9 rounded-full bg-zinc-100 flex items-center justify-center shrink-0">
                        <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M16.667 8.33c0 4.162-4.616 8.495-6.166 9.833a.83.83 0 0 1-1.002 0c-1.55-1.338-6.166-5.671-6.166-9.832a6.667 6.667 0 0 1 13.334 0" stroke="#71717b" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/><path d="M10 10.836a2.5 2.5 0 1 0 0-5 2.5 2.5 0 0 0 0 5" stroke="#71717b" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
                    </div>
                    <span class="text-sm text-zinc-600">2425 HSR Layout, Bangalore, TX73301</span>
                </div>
            </div>
        </div>

        <div class="border border-zinc-200 rounded-2xl p-6 md:p-8 w-full max-w-[470px] mx-auto md:ml-auto md:mr-0">
            <form class="flex flex-col space-y-6">
                
                <div class="flex flex-col space-y-2">
                    <label class="text-sm text-zinc-700">Full Name</label>
                    <input type="text" placeholder="Enter your name" class="rounded-full border border-zinc-200 px-4 py-2.5 text-sm text-zinc-900 placeholder:text-zinc-500 focus:outline-none focus:border-zinc-400" />
                </div>

                <div class="flex flex-col space-y-2">
                    <label class="text-sm text-zinc-700">Email address</label>
                    <input type="email" placeholder="Enter you email" class="rounded-full border border-zinc-200 px-4 py-2.5 text-sm text-zinc-900 placeholder:text-zinc-500 focus:outline-none focus:border-zinc-400" />
                </div>

                <div class="flex flex-col space-y-2">
                    <label class="text-sm text-zinc-700">Message</label>
                    <textarea placeholder="Enter your message" class="rounded-xl border border-zinc-200 px-4 py-3 text-sm text-zinc-900 placeholder:text-zinc-500 focus:outline-none focus:border-zinc-400 h-24 resize-none"></textarea>
                </div>

                <div class="flex items-center gap-2">
                    <div class="size-3.5 rounded-full border border-zinc-200 shrink-0 cursor-pointer flex items-center justify-center"></div>
                    <span class="text-xs text-zinc-950">
                        I agree with <a href="#" class="text-xs text-zinc-700 underline hover:text-zinc-900">the terms and conditions</a>
                    </span>
                </div>

                <button class="w-full bg-zinc-950 text-white text-sm py-3 rounded-full hover:bg-zinc-800 transition-colors cursor-pointer">
                    Submit
                </button>
            </form>
        </div>

    </div>
</div>

  </section>
</template>