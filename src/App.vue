<template>
  <div class="bg-[#111827] min-h-screen">
    <NavBar />
    <HeroSection />
    <ServicesSection />
    <AboutSection />
    <ExperienceAndSkills />
    <LatestProjSection />
    <ContactSection />
    <TestimonialsSection />
    <Footer />
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
const TestimonialsSection = defineAsyncComponent(() => import('@/components/TestimonialsSection.vue'))
const ContactSection = defineAsyncComponent(() => import('@/components/ContactSection.vue'))
const LatestProjSection = defineAsyncComponent(() => import('@/components/LatestProjSection.vue'))
const Footer = defineAsyncComponent(() => import('@/components/Footer.vue'))
</script>