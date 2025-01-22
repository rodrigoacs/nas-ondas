<template>
  <HeaderSection class="header-section" />
  <HomeSection id="home" />
  <!-- <NewsSection id="news" /> -->
  <InterviewSection id="interview" />
  <!-- <EventSection id="event" /> -->
  <AboutSection id="about" />
  <ContactSection id="contact" />
  <FooterSection class="footer" />
</template>

<script setup>
import HeaderSection from './components/HeaderSection.vue'
import HomeSection from './components/HomeSection.vue'
import NewsSection from './components/NewsSection.vue'
import InterviewSection from './components/InterviewSection.vue'
import EventSection from './components/EventSection.vue'
import AboutSection from './components/AboutSection.vue'
import ContactSection from './components/ContactSection.vue'
import FooterSection from './components/FooterSection.vue'

</script>

<style scoped>
.header-section {
  position: sticky;
  top: 0;
  z-index: 100;
}
</style>
