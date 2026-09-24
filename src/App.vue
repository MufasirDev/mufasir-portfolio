<script setup lang="ts">
import { onMounted, onUnmounted } from 'vue'

import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import Skills from './components/Skills.vue'
import Projects from './components/Projects.vue'
import Experience from './components/Experience.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'

let observer: IntersectionObserver | null = null

onMounted(() => {
  const elements = document.querySelectorAll(
    '.about-section, .skills-section, .projects-section, .experience-section, .contact-section'
  )

  observer = new IntersectionObserver(
    (entries) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          entry.target.classList.add('section-visible')
          observer?.unobserve(entry.target)
        }
      })
    },
    {
      threshold: 0.12,
    }
  )

  elements.forEach((element) => {
    element.classList.add('section-hidden')
    observer?.observe(element)
  })
})

onUnmounted(() => {
  observer?.disconnect()
})
</script>

<template>
  <Navbar />

  <main>
    <Hero />
    <About />
    <Skills />
    <Projects />
    <Experience />
    <Contact />
  </main>

  <Footer />
</template>

<style>
/* =================================
   SECTION REVEAL ANIMATION
================================= */

.section-hidden {
  opacity: 0;
  transform: translateY(35px);
  transition:
    opacity 0.8s ease,
    transform 0.8s ease;
}

.section-visible {
  opacity: 1;
  transform: translateY(0);
}


/* =================================
   ACCESSIBILITY
================================= */

@media (prefers-reduced-motion: reduce) {
  .section-hidden,
  .section-visible {
    opacity: 1;
    transform: none;
    transition: none;
  }
}
</style>