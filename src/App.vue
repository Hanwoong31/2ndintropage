<template>
  <HeroSection />
  <CareerSection />
  <ContactSection />
</template>

<script setup>
import HeroSection from './components/HeroSection.vue'
import CareerSection from './components/CareerSection.vue'
import ContactSection from './components/ContactSection.vue'
</script>

<style>
html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  font-family: 'Noto Sans KR', sans-serif;
  background-color: #fdfdfd;
}
</style>
