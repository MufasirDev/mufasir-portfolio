<script setup lang="ts">
import profileImage from '../assets/profile.jpg'
</script>

<template>
  <section id="home" class="hero">
    <div class="hero-container">

      <!-- LEFT SIDE -->
      <div class="hero-content">

        <p class="eyebrow">
          FRONTEND DEVELOPER • FINTECH BUILDER
        </p>

        <h1>
          Hi, I'm
          <span>Adebayo Muh'sin</span>
          Adebola
        </h1>

        <h2>
          Frontend Developer & Banking and Finance Student
        </h2>

        <p class="hero-text">
          I create modern, responsive and user-friendly digital experiences
          while combining technology, creativity and financial knowledge.
          I'm passionate about building digital products that solve
          real-world problems.
        </p>

        <div class="hero-buttons">
          <a href="#projects" class="primary-btn">
            View My Work
          </a>

          <a href="#contact" class="secondary-btn">
            Contact Me
          </a>
        </div>

        <div class="social-links">
          <a
            href="https://github.com/"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="GitHub"
          >
            GitHub
          </a>

          <a
            href="https://www.linkedin.com/"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="LinkedIn"
          >
            LinkedIn
          </a>

          <a
            href="https://wa.me/2348093963715"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="WhatsApp"
          >
            WhatsApp
          </a>
        </div>

      </div>

      <!-- RIGHT SIDE -->
      <div class="hero-visual">

        <div class="hero-glow glow-one"></div>
        <div class="hero-glow glow-two"></div>

        <!-- PROFILE PHOTO -->
        <div class="profile-frame">
          <div class="profile-inner">

            <img
              :src="profileImage"
              alt="Adebayo Muh'sin Adebola"
              class="profile-image"
            />

          </div>
        </div>

        <!-- FLOATING CARDS -->
        <div class="floating-card card-top">
          <span>01</span>
          <p>Frontend Developer</p>
        </div>

        <div class="floating-card card-bottom">
          <span>02</span>
          <p>Fintech Builder</p>
        </div>

      </div>

    </div>
  </section>
</template>

<style scoped>
.hero {
  min-height: 100vh;
  padding: 150px 7% 80px;
  display: flex;
  align-items: center;
  position: relative;
  overflow: hidden;
}

.hero-container {
  width: 100%;
  max-width: 1300px;
  margin: 0 auto;

  display: grid;
  grid-template-columns: 1.05fr 0.95fr;
  align-items: center;
  gap: 70px;
}

/* =========================
   LEFT SIDE
========================= */

.hero-content {
  max-width: 720px;
}

.eyebrow {
  color: #3b82f6;
  font-size: 13px;
  font-weight: 800;
  letter-spacing: 3px;
  margin-bottom: 22px;
}

.hero h1 {
  margin: 0;
  font-size: clamp(48px, 6vw, 78px);
  line-height: 1.05;
  font-weight: 900;
  letter-spacing: -2px;
  color: #ffffff;
}

.hero h1 span {
  display: block;
  color: #3b82f6;
}

.hero h2 {
  margin-top: 25px;
  color: #cbd5e1;
  font-size: clamp(20px, 2.2vw, 28px);
  line-height: 1.4;
  font-weight: 700;
}

.hero-text {
  max-width: 650px;
  margin-top: 22px;
  color: #94a3b8;
  font-size: 17px;
  line-height: 1.8;
}

/* =========================
   BUTTONS
========================= */

.hero-buttons {
  display: flex;
  gap: 16px;
  margin-top: 35px;
  flex-wrap: wrap;
}

.primary-btn,
.secondary-btn {
  text-decoration: none;
  padding: 15px 25px;
  border-radius: 10px;
  font-weight: 800;
  transition: 0.3s ease;
}

.primary-btn {
  color: white;
  background: #2563eb;
  box-shadow: 0 12px 30px rgba(37, 99, 235, 0.25);
}

.primary-btn:hover {
  background: #1d4ed8;
  transform: translateY(-3px);
}

.secondary-btn {
  color: white;
  border: 1px solid rgba(255, 255, 255, 0.15);
  background: rgba(255, 255, 255, 0.04);
}

.secondary-btn:hover {
  border-color: #3b82f6;
  transform: translateY(-3px);
}

/* =========================
   SOCIAL LINKS
========================= */

.social-links {
  display: flex;
  gap: 24px;
  margin-top: 35px;
}

.social-links a {
  color: #94a3b8;
  text-decoration: none;
  font-size: 14px;
  font-weight: 700;
  transition: 0.3s ease;
}

.social-links a:hover {
  color: #3b82f6;
}

/* =========================
   RIGHT SIDE
========================= */

.hero-visual {
  min-height: 560px;
  position: relative;

  display: flex;
  align-items: center;
  justify-content: center;
}

/* =========================
   PROFILE FRAME
========================= */

.profile-frame {
  width: 390px;
  height: 470px;

  padding: 8px;
  border-radius: 30px;

  background: linear-gradient(
    145deg,
    #3b82f6,
    #1d4ed8,
    #172554
  );

  transform: rotate(3deg);

  box-shadow:
    0 30px 80px rgba(37, 99, 235, 0.25),
    0 0 80px rgba(37, 99, 235, 0.12);

  position: relative;
  z-index: 2;
}

.profile-inner {
  width: 100%;
  height: 100%;

  border-radius: 24px;
  overflow: hidden;

  background: #080f23;

  display: flex;
  align-items: center;
  justify-content: center;
}

/* =========================
   PROFILE IMAGE
========================= */

.profile-image {
  width: 100%;
  height: 100%;

  object-fit: cover;
  display: block;

  transform: rotate(-3deg) scale(1.02);
}

/* =========================
   GLOW
========================= */

.hero-glow {
  position: absolute;
  border-radius: 50%;
  filter: blur(70px);
  pointer-events: none;
}

.glow-one {
  width: 220px;
  height: 220px;

  background: rgba(37, 99, 235, 0.25);

  top: 50px;
  right: 70px;
}

.glow-two {
  width: 180px;
  height: 180px;

  background: rgba(59, 130, 246, 0.15);

  bottom: 50px;
  left: 70px;
}

/* =========================
   FLOATING CARDS
========================= */

.floating-card {
  position: absolute;
  z-index: 5;

  padding: 15px 18px;

  display: flex;
  align-items: center;
  gap: 12px;

  border: 1px solid rgba(255, 255, 255, 0.08);

  background: rgba(8, 15, 35, 0.88);

  backdrop-filter: blur(15px);

  border-radius: 12px;

  box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);

  animation: floating 4s ease-in-out infinite;
}

.floating-card span {
  color: #3b82f6;
  font-size: 12px;
  font-weight: 900;
}

.floating-card p {
  margin: 0;
  color: #e2e8f0;
  font-size: 13px;
  font-weight: 700;
}

.card-top {
  top: 90px;
  right: -15px;
}

.card-bottom {
  bottom: 80px;
  left: -20px;
  animation-delay: 1.5s;
}

/* =========================
   FLOATING ANIMATION
========================= */

@keyframes floating {
  0%,
  100% {
    transform: translateY(0);
  }

  50% {
    transform: translateY(-8px);
  }
}

/* =========================
   TABLET
========================= */

@media (max-width: 1000px) {
  .hero-container {
    grid-template-columns: 1fr;
    text-align: center;
  }

  .hero-content {
    margin: 0 auto;
  }

  .hero-text {
    margin-left: auto;
    margin-right: auto;
  }

  .hero-buttons,
  .social-links {
    justify-content: center;
  }

  .hero-visual {
    margin-top: 20px;
  }
}

/* =========================
   MOBILE
========================= */

@media (max-width: 600px) {
  .hero {
    padding: 130px 5% 60px;
  }

  .hero h1 {
    font-size: clamp(42px, 12vw, 58px);
    letter-spacing: -1.5px;
  }

  .hero h2 {
    font-size: 20px;
  }

  .hero-text {
    font-size: 15px;
  }

  .profile-frame {
    width: 300px;
    height: 390px;
  }

  .hero-visual {
    min-height: 450px;
  }

  .card-top {
    right: 0;
  }

  .card-bottom {
    left: 0;
  }

  .floating-card {
    padding: 12px 14px;
  }

  .floating-card p {
    font-size: 12px;
  }
}

/* =========================
   SMALL PHONES
========================= */

@media (max-width: 380px) {
  .profile-frame {
    width: 270px;
    height: 350px;
  }

  .card-top {
    top: 65px;
  }

  .card-bottom {
    bottom: 55px;
  }

  .floating-card {
    transform: scale(0.9);
  }
}
</style>