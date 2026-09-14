<template>
  <section id="projects" class="projects-section">
    <div class="projects-container">

      <div class="section-heading">
        <span>MY PROJECTS</span>
        <h2>Things I've built with technology.</h2>
        <p>
          A selection of projects that showcase my frontend development
          skills and interest in solving real-world problems.
        </p>
      </div>

      <div class="projects-grid">

        <!-- PROJECT 1 -->
        <article class="project-card featured">
          <div class="project-top">
            <div class="project-icon">M</div>

            <span class="project-status">
              Featured
            </span>
          </div>

          <div class="project-content">
            <span class="project-type">
              Education Platform
            </span>

            <h3>Mufasir Devmaster Academy</h3>

            <p>
              A modern learning platform designed to help students learn
              frontend development through practical and structured
              courses.
            </p>

            <div class="tech-stack">
              <span>Vue.js</span>
              <span>Vite</span>
              <span>Supabase</span>
              <span>Paystack</span>
            </div>
          </div>

          <div class="project-footer">
            <a href="#" class="project-link">
              View Project
              <span>→</span>
            </a>
          </div>
        </article>

        <!-- PROJECT 2 -->
        <article class="project-card">
          <div class="project-top">
            <div class="project-icon">B</div>

            <span class="project-number">
              02
            </span>
          </div>

          <div class="project-content">
            <span class="project-type">
              Fintech / Banking
            </span>

            <h3>BankScope</h3>

            <p>
              A banking interface concept focused on account management,
              dashboards, transactions and personal financial tracking.
            </p>

            <div class="tech-stack">
              <span>Vue.js</span>
              <span>Vite</span>
              <span>JavaScript</span>
            </div>
          </div>

          <div class="project-footer">
            <a href="#" class="project-link">
              View Project
              <span>→</span>
            </a>
          </div>
        </article>

        <!-- PROJECT 3 -->
        <article class="project-card">
          <div class="project-top">
            <div class="project-icon">F</div>

            <span class="project-number">
              03
            </span>
          </div>

          <div class="project-content">
            <span class="project-type">
              Open Banking
            </span>

            <h3>FinView</h3>

            <p>
              A financial dashboard concept featuring accounts,
              transactions, transfers, analytics and user profile
              management.
            </p>

            <div class="tech-stack">
              <span>Vue.js</span>
              <span>Vite</span>
              <span>CSS</span>
            </div>
          </div>

          <div class="project-footer">
            <a href="#" class="project-link">
              View Project
              <span>→</span>
            </a>
          </div>
        </article>

      </div>

      <div class="projects-bottom">
        <p>
          More projects coming soon.
        </p>
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

/* HEADING */

.section-heading {
  max-width: 800px;
  margin-bottom: 60px;
}

.section-heading span {
  color: #3b82f6;
  font-size: 13px;
  font-weight: 800;
  letter-spacing: 3px;
}

.section-heading h2 {
  margin: 15px 0 18px;

  color: #ffffff;
  font-size: clamp(36px, 5vw, 58px);
  line-height: 1.1;
  font-weight: 900;
}

.section-heading p {
  max-width: 650px;

  color: #94a3b8;
  font-size: 16px;
  line-height: 1.8;
}

/* GRID */

.projects-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 22px;
}

/* CARD */

.project-card {
  position: relative;

  min-height: 440px;
  padding: 30px;

  display: flex;
  flex-direction: column;

  border: 1px solid rgba(255, 255, 255, 0.07);
  border-radius: 20px;

  background: rgba(255, 255, 255, 0.025);

  transition: 0.35s ease;
}

.project-card:hover {
  transform: translateY(-8px);

  border-color: rgba(59, 130, 246, 0.4);

  box-shadow:
    0 25px 60px rgba(0, 0, 0, 0.25),
    0 0 30px rgba(37, 99, 235, 0.05);
}

.project-card.featured {
  grid-row: span 2;

  min-height: 650px;

  background:
    linear-gradient(
      145deg,
      rgba(37, 99, 235, 0.13),
      rgba(255, 255, 255, 0.025)
    );
}

/* TOP */

.project-top {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.project-icon {
  width: 58px;
  height: 58px;

  display: flex;
  align-items: center;
  justify-content: center;

  border-radius: 15px;

  background: rgba(37, 99, 235, 0.12);

  color: #3b82f6;

  font-size: 24px;
  font-weight: 900;
}

.project-status,
.project-number {
  color: #64748b;
  font-size: 12px;
  font-weight: 800;
  letter-spacing: 1px;
}

.project-status {
  padding: 7px 11px;

  color: #60a5fa;

  border: 1px solid rgba(59, 130, 246, 0.2);
  border-radius: 30px;

  background: rgba(37, 99, 235, 0.08);
}

/* CONTENT */

.project-content {
  margin-top: 45px;
}

.project-type {
  color: #3b82f6;

  font-size: 12px;
  font-weight: 800;
  letter-spacing: 1.5px;
  text-transform: uppercase;
}

.project-content h3 {
  margin: 12px 0 15px;

  color: #ffffff;

  font-size: 28px;
  font-weight: 900;
}

.project-content p {
  color: #94a3b8;

  font-size: 15px;
  line-height: 1.8;
}

/* TECHNOLOGIES */

.tech-stack {
  display: flex;
  flex-wrap: wrap;
  gap: 9px;

  margin-top: 25px;
}

.tech-stack span {
  padding: 7px 11px;

  border-radius: 6px;

  color: #cbd5e1;

  background: rgba(255, 255, 255, 0.05);

  font-size: 11px;
  font-weight: 700;
}

/* FOOTER */

.project-footer {
  margin-top: auto;

  padding-top: 30px;
}

.project-link {
  display: inline-flex;
  align-items: center;
  gap: 10px;

  color: #ffffff;

  text-decoration: none;

  font-size: 14px;
  font-weight: 800;

  transition: 0.3s ease;
}

.project-link span {
  color: #3b82f6;
  font-size: 20px;

  transition: 0.3s ease;
}

.project-link:hover {
  color: #3b82f6;
}

.project-link:hover span {
  transform: translateX(5px);
}

/* BOTTOM */

.projects-bottom {
  margin-top: 45px;

  text-align: center;
}

.projects-bottom p {
  color: #64748b;
  font-size: 14px;
}

/* RESPONSIVE */

@media (max-width: 850px) {
  .projects-grid {
    grid-template-columns: 1fr;
  }

  .project-card.featured {
    grid-row: auto;
    min-height: 440px;
  }
}

@media (max-width: 600px) {
  .projects-section {
    padding: 90px 5%;
  }

  .project-card {
    min-height: 400px;
    padding: 25px;
  }

  .project-content h3 {
    font-size: 24px;
  }
}
</style>