<script setup lang="ts">
import { ref } from 'vue'

const menuOpen = ref(false)

const closeMenu = () => {
  menuOpen.value = false
}
</script>

<template>
  <nav class="navbar">

    <div class="nav-container">

      <!-- LOGO -->
      <a
        href="#home"
        class="logo"
        @click="closeMenu"
      >
        <span>M</span>ufasir
      </a>


      <!-- DESKTOP NAVIGATION -->
      <div class="nav-links">

        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#experience">Journey</a>
        <a href="#contact">Contact</a>

      </div>


      <!-- DESKTOP BUTTON -->
      <a
        href="#contact"
        class="nav-button"
      >
        Let's Talk
      </a>


      <!-- MOBILE MENU BUTTON -->
      <button
        class="menu-button"
        :class="{ active: menuOpen }"
        @click="menuOpen = !menuOpen"
        aria-label="Toggle navigation menu"
        :aria-expanded="menuOpen"
      >
        <span></span>
        <span></span>
        <span></span>
      </button>

    </div>


    <!-- MOBILE NAVIGATION -->
    <div
      class="mobile-menu"
      :class="{ open: menuOpen }"
    >

      <a
        href="#home"
        @click="closeMenu"
      >
        Home
      </a>

      <a
        href="#about"
        @click="closeMenu"
      >
        About
      </a>

      <a
        href="#skills"
        @click="closeMenu"
      >
        Skills
      </a>

      <a
        href="#projects"
        @click="closeMenu"
      >
        Projects
      </a>

      <a
        href="#experience"
        @click="closeMenu"
      >
        Journey
      </a>

      <a
        href="#contact"
        @click="closeMenu"
      >
        Contact
      </a>

      <a
        href="#contact"
        class="mobile-talk"
        @click="closeMenu"
      >
        Let's Talk
      </a>

    </div>

  </nav>
</template>


<style scoped>
/* =================================
   NAVBAR
================================= */

.navbar {
  position: fixed;

  top: 0;
  left: 0;

  width: 100%;

  z-index: 1000;

  padding: 20px 7%;

  background: rgba(5, 10, 25, 0.88);

  backdrop-filter: blur(16px);

  -webkit-backdrop-filter: blur(16px);

  border-bottom: 1px solid rgba(255, 255, 255, 0.06);
}


/* =================================
   NAV CONTAINER
================================= */

.nav-container {
  max-width: 1300px;

  margin: 0 auto;

  display: flex;

  align-items: center;

  justify-content: space-between;
}


/* =================================
   LOGO
================================= */

.logo {
  color: #ffffff;

  font-size: 28px;

  font-weight: 900;

  text-decoration: none;

  letter-spacing: -1px;
}

.logo span {
  color: #3b82f6;
}


/* =================================
   DESKTOP LINKS
================================= */

.nav-links {
  display: flex;

  align-items: center;

  gap: 30px;
}

.nav-links a {
  position: relative;

  color: #cbd5e1;

  text-decoration: none;

  font-size: 14px;

  font-weight: 700;

  transition: 0.3s ease;
}

.nav-links a::after {
  content: '';

  position: absolute;

  left: 0;
  bottom: -7px;

  width: 0;
  height: 2px;

  background: #3b82f6;

  transition: 0.3s ease;
}

.nav-links a:hover {
  color: #ffffff;
}

.nav-links a:hover::after {
  width: 100%;
}


/* =================================
   TALK BUTTON
================================= */

.nav-button {
  padding: 11px 20px;

  color: #ffffff;

  background: #2563eb;

  border-radius: 8px;

  text-decoration: none;

  font-size: 13px;

  font-weight: 800;

  transition: 0.3s ease;
}

.nav-button:hover {
  background: #1d4ed8;

  transform: translateY(-2px);
}


/* =================================
   MOBILE BUTTON
================================= */

.menu-button {
  display: none;

  width: 42px;
  height: 42px;

  padding: 0;

  border: 1px solid rgba(255, 255, 255, 0.1);

  border-radius: 9px;

  background: rgba(255, 255, 255, 0.04);

  cursor: pointer;

  align-items: center;
  justify-content: center;

  flex-direction: column;

  gap: 5px;
}

.menu-button span {
  width: 19px;
  height: 2px;

  border-radius: 2px;

  background: #ffffff;

  transition: 0.3s ease;
}


/* =================================
   HAMBURGER ANIMATION
================================= */

.menu-button.active span:nth-child(1) {
  transform: translateY(7px) rotate(45deg);
}

.menu-button.active span:nth-child(2) {
  opacity: 0;
}

.menu-button.active span:nth-child(3) {
  transform: translateY(-7px) rotate(-45deg);
}


/* =================================
   MOBILE MENU
================================= */

.mobile-menu {
  display: none;
}


/* =================================
   TABLET / MOBILE
================================= */

@media (max-width: 850px) {

  .navbar {
    padding: 17px 5%;
  }

  .nav-links,
  .nav-button {
    display: none;
  }

  .menu-button {
    display: flex;
  }

  .mobile-menu {
    display: flex;

    position: absolute;

    top: 100%;

    left: 5%;
    right: 5%;

    padding: 15px;

    flex-direction: column;

    gap: 5px;

    background: rgba(7, 13, 31, 0.98);

    border: 1px solid rgba(255, 255, 255, 0.08);

    border-radius: 14px;

    box-shadow:
      0 20px 50px rgba(0, 0, 0, 0.4);

    opacity: 0;

    visibility: hidden;

    transform: translateY(-10px);

    pointer-events: none;

    transition:
      opacity 0.25s ease,
      transform 0.25s ease,
      visibility 0.25s ease;
  }

  .mobile-menu.open {
    opacity: 1;

    visibility: visible;

    transform: translateY(0);

    pointer-events: auto;
  }

  .mobile-menu a {
    padding: 13px 15px;

    color: #cbd5e1;

    text-decoration: none;

    border-radius: 8px;

    font-size: 14px;

    font-weight: 700;

    transition: 0.3s ease;
  }

  .mobile-menu a:hover {
    color: #ffffff;

    background: rgba(37, 99, 235, 0.1);
  }

  .mobile-menu .mobile-talk {
    margin-top: 7px;

    text-align: center;

    color: #ffffff;

    background: #2563eb;
  }

  .mobile-menu .mobile-talk:hover {
    background: #1d4ed8;
  }
}


/* =================================
   SMALL PHONES
================================= */

@media (max-width: 400px) {

  .logo {
    font-size: 25px;
  }

  .menu-button {
    width: 39px;
    height: 39px;
  }

}
</style>