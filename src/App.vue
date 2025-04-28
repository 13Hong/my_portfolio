<template>
  <div class="bg-[#111827] min-h-screen">
    <NavBar />
    <HeroSection />
    <ServicesSection />
    <AboutSection />
    <ExperienceAndSkills />
    <LatestProjSection />
  </div>
</template>

<script setup>
import { defineAsyncComponent } from 'vue';
// Import Conpoments Asynchronously
const NavBar = defineAsyncComponent(() => import('@/components/NavBar.vue'))
const HeroSection = defineAsyncComponent(() => import('@/components/HeroSection.vue'))
const ServicesSection = defineAsyncComponent(() => import('@/components/ServicesSection.vue'))
const AboutSection = defineAsyncComponent(() => import('@/components/AboutSection.vue'))
const ExperienceAndSkills = defineAsyncComponent(() => import('@/components/ExperienceAndSkills.vue'))
const LatestProjSection = defineAsyncComponent(() => import('@/components/LatestProjSection.vue'))
</script>