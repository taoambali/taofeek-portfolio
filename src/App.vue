<template>
  <div class="bg-[#111827] min-h-screen">
    <NavBar />
    <HeroSection />
    <Services />
    <About />
    <Skills />
    <Contact />
  </div>
</template>
<script setup>
import NavBar from "@/components/Navbar.vue";
import HeroSection from "@/components/HeroSection.vue";
import Services from "./components/Services.vue";
import About from "./components/About.vue";
import Skills from "./components/Skills.vue";
import Contact from "./components/Contact.vue";
</script>
<style></style>
