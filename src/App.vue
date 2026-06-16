<script setup>
import { ref } from "vue";

import Navbar from "./components/Navbar.vue";
import HeroSection from "./components/sections/HeroSection.vue";
import AboutSection from "./components/sections/AboutSection.vue";
import SkillsSection from "./components/sections/SkillsSection.vue";
import ProjectsSection from "./components/sections/ProjectsSection.vue";
import EducationSection from "./components/sections/EducationSection.vue";
import ExperienceSection from "./components/sections/ExperienceSection.vue";
import ContactSection from "./components/sections/ContactSection.vue";
import FooterSection from "./components/sections/FooterSection.vue";
import CVModal from "./components/CVModal.vue";

const showCV = ref(false);

function openCV() {
  showCV.value = true;
}

function closeCV() {
  showCV.value = false;
}
</script>

<template>

  <HeroSection @open-cv="openCV"/>

  <CVModal :is-open="showCV" @close="closeCV" />

  <AboutSection />

  <SkillsSection />

  <ProjectsSection />

  <EducationSection />

  <ExperienceSection />

  <ContactSection />

  <FooterSection />
</template>
