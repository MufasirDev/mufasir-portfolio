<template>
  <section id="projects" class="projects-section">
    <div class="projects-container">

      <!-- SECTION HEADER -->
      <div class="section-heading">
        <span>MY PROJECTS</span>

        <h2>
          Things I've built with
          <span>technology.</span>
        </h2>

        <p>
          A selection of projects I've worked on across fintech,
          education, business and modern web development.
        </p>
      </div>

      <!-- PROJECTS -->
      <div class="projects-grid">

        <!-- MUFASIRPAY -->
        <article class="project-card featured">

          <div class="project-top">
            <div class="project-number">01</div>

            <span class="project-status">
              Fintech
            </span>
          </div>

          <div class="project-content">

            <h3>MufasirPay</h3>

            <p class="project-description">
              A fintech and digital wallet platform designed to provide
              users with a modern experience for managing wallets,
              transfers, airtime, data, bills and transactions.
            </p>

            <div class="project-tags">
              <span>Vue.js</span>
              <span>Vite</span>
              <span>Supabase</span>
              <span>Paystack</span>
            </div>

            <div class="project-links">
  <a
    href="https://mufasirpay.vercel.app/"
    target="_blank"
    rel="noopener noreferrer"
    class="project-link"
  >
    Live Project
    <span>↗</span>
  </a>
</div>

          </div>

        </article>

        <!-- MUFASIR DEVMaster -->
        <article class="project-card">

          <div class="project-top">
            <div class="project-number">02</div>

            <span class="project-status">
              Education
            </span>
          </div>

          <div class="project-content">

            <h3>Mufasir Devmaster Academy</h3>

            <p class="project-description">
              A learning platform created to provide web development
              education and digital learning experiences for students
              interested in technology.
            </p>

            <div class="project-tags">
              <span>Vue.js</span>
              <span>Vite</span>
              <span>Supabase</span>
              <span>Paystack</span>
            </div>

            <div class="project-links">
  <a
    href="https://mufasirdev.vercel.app/"
    target="_blank"
    rel="noopener noreferrer"
    class="project-link"
  >
    Live Project
    <span>↗</span>
  </a>
</div>

          </div>

        </article>

        <!-- FINVIEW -->
        <article class="project-card">

          <div class="project-top">
            <div class="project-number">03</div>

            <span class="project-status">
              Open Banking
            </span>
          </div>

          <div class="project-content">

            <h3>FinView</h3>

            <p class="project-description">
              An open banking dashboard concept focused on helping
              users visualize financial accounts, transactions,
              transfers and financial insights in one place.
            </p>

            <div class="project-tags">
              <span>Vue.js</span>
              <span>Vite</span>
              <span>JavaScript</span>
              <span>CSS</span>
            </div>

            <div class="project-links">
  <a
    href="https://finview1.netlify.app/"
    target="_blank"
    rel="noopener noreferrer"
    class="project-link"
  >
    Live Project
    <span>↗</span>
  </a>
</div>

          </div>

        </article>

        

        <!-- FARFAD KITCHEN -->
        <article class="project-card">

          <div class="project-top">
            <div class="project-number">05</div>

            <span class="project-status">
              Business
            </span>
          </div>

          <div class="project-content">

            <h3>Farfad Kitchen</h3>

            <p class="project-description">
              A responsive restaurant website designed to showcase
              food menus, special offers, gallery content and make it
              easier for customers to place orders.
            </p>

            <div class="project-tags">
              <span>Vue.js</span>
              <span>Vite</span>
              <span>CSS</span>
              <span>WhatsApp</span>
            </div>

            <div class="project-links">
  <a
    href="https://realfarfadkitchen.com/"
    target="_blank"
    rel="noopener noreferrer"
    class="project-link"
  >
    Live Project
    <span>↗</span>
  </a>
</div>

          </div>

        </article>

       

          </div>


      </div>

  </section>
</template>

<style scoped>
.projects-section {
  padding: 120px 7%;
  background: #070d1f;
}

.projects-container {
  max-width: 1200px;
  margin: 0 auto;
}

/* =========================
   SECTION HEADER
========================= */

.section-heading {
  max-width: 850px;
  margin-bottom: 65px;
}

.section-heading > span {
  color: #3b82f6;
  font-size: 13px;
  font-weight: 800;
  letter-spacing: 3px;
}

.section-heading h2 {
  margin-top: 15px;

  color: #ffffff;

  font-size: clamp(36px, 5vw, 58px);
  line-height: 1.1;

  font-weight: 900;
  letter-spacing: -1.5px;
}

.section-heading h2 span {
  color: #3b82f6;
}

.section-heading p {
  max-width: 700px;
  margin-top: 20px;

  color: #94a3b8;

  font-size: 16px;
  line-height: 1.8;
}

/* =========================
   PROJECT GRID
========================= */

.projects-grid {
  display: grid;

  grid-template-columns: repeat(2, 1fr);

  gap: 22px;
}

/* =========================
   PROJECT CARD
========================= */

.project-card {
  min-height: 390px;

  padding: 32px;

  display: flex;
  flex-direction: column;

  border: 1px solid rgba(255, 255, 255, 0.07);

  border-radius: 20px;

  background: rgba(255, 255, 255, 0.025);

  position: relative;

  overflow: hidden;

  transition: 0.35s ease;
}

.project-card::before {
  content: '';

  position: absolute;

  width: 240px;
  height: 240px;

  top: -130px;
  right: -120px;

  border-radius: 50%;

  background: rgba(37, 99, 235, 0.08);

  filter: blur(40px);

  transition: 0.35s ease;
}

.project-card:hover {
  transform: translateY(-8px);

  border-color: rgba(59, 130, 246, 0.4);

  box-shadow:
    0 30px 70px rgba(0, 0, 0, 0.25);
}

.project-card:hover::before {
  background: rgba(37, 99, 235, 0.17);
}

/* FEATURED */

.project-card.featured {
  border-color: rgba(59, 130, 246, 0.25);

  background:
    linear-gradient(
      145deg,
      rgba(37, 99, 235, 0.08),
      rgba(255, 255, 255, 0.025)
    );
}

/* =========================
   TOP
========================= */

.project-top {
  display: flex;

  align-items: center;

  justify-content: space-between;
}

.project-number {
  color: #3b82f6;

  font-size: 13px;

  font-weight: 900;

  letter-spacing: 2px;
}

.project-status {
  padding: 7px 11px;

  border-radius: 20px;

  color: #93c5fd;

  background: rgba(37, 99, 235, 0.1);

  border: 1px solid rgba(59, 130, 246, 0.15);

  font-size: 11px;

  font-weight: 800;
}

/* =========================
   CONTENT
========================= */

.project-content {
  margin-top: 55px;

  position: relative;

  z-index: 2;
}

.project-content h3 {
  color: #ffffff;

  font-size: 25px;

  font-weight: 900;

  line-height: 1.25;
}

.project-description {
  margin-top: 15px;

  color: #94a3b8;

  font-size: 14px;

  line-height: 1.8;
}

/* =========================
   TAGS
========================= */

.project-tags {
  display: flex;

  flex-wrap: wrap;

  gap: 8px;

  margin-top: 24px;
}

.project-tags span {
  padding: 7px 10px;

  border-radius: 7px;

  color: #cbd5e1;

  background: rgba(255, 255, 255, 0.04);

  border: 1px solid rgba(255, 255, 255, 0.07);

  font-size: 11px;

  font-weight: 700;
}

/* =========================
   LINKS
========================= */

.project-links {
  margin-top: 28px;
}

.project-link {
  display: inline-flex;

  align-items: center;

  gap: 8px;

  color: #3b82f6;

  text-decoration: none;

  font-size: 14px;

  font-weight: 800;

  transition: 0.3s ease;
}

.project-link span {
  font-size: 18px;

  transition: 0.3s ease;
}

.project-link:hover {
  color: #60a5fa;
}

.project-link:hover span {
  transform: translate(4px, -4px);
}

/* =========================
   TABLET
========================= */

@media (max-width: 850px) {
  .projects-grid {
    grid-template-columns: 1fr;
  }
}

/* =========================
   MOBILE
========================= */

@media (max-width: 550px) {
  .projects-section {
    padding: 90px 5%;
  }

  .project-card {
    min-height: auto;

    padding: 25px;
  }

  .project-content {
    margin-top: 40px;
  }

  .project-content h3 {
    font-size: 22px;
  }

  .section-heading h2 {
    font-size: 38px;
  }
}
</style>