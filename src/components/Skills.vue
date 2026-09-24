<template>
  <section id="skills" class="skills-section">
    <div class="skills-container">

      <!-- SECTION HEADER -->
      <div class="section-heading">
        <span>MY SKILLS</span>

        <h2>
          Technologies I use to
          <span>build digital products.</span>
        </h2>

        <p>
          A combination of frontend development, backend services,
          fintech technologies and developer tools that I use while
          building and experimenting with digital products.
        </p>
      </div>

      <!-- SKILL CATEGORIES -->
      <div class="skills-grid">

        <!-- FRONTEND -->
        <div class="skill-card">
          <div class="skill-icon">
            &lt;/&gt;
          </div>

          <h3>Frontend Development</h3>

          <p>
            Building responsive, modern and interactive user interfaces.
          </p>

          <div class="skill-tags">
            <span>HTML5</span>
            <span>CSS3</span>
            <span>JavaScript</span>
            <span>Vue.js</span>
            <span>Vite</span>
            <span>Responsive Design</span>
          </div>
        </div>

        <!-- BACKEND -->
        <div class="skill-card">
          <div class="skill-icon">
            { }
          </div>

          <h3>Backend & Database</h3>

          <p>
            Working with backend services and databases to power
            modern web applications.
          </p>

          <div class="skill-tags">
            <span>Supabase</span>
            <span>PostgreSQL</span>
            <span>Authentication</span>
            <span>RLS</span>
            <span>Edge Functions</span>
          </div>
        </div>

        <!-- FINTECH -->
        <div class="skill-card">
          <div class="skill-icon">
            ₦
          </div>

          <h3>Fintech Development</h3>

          <p>
            Building and exploring digital financial products,
            payment systems and fintech experiences.
          </p>

          <div class="skill-tags">
            <span>Paystack</span>
            <span>Digital Wallets</span>
            <span>Transactions</span>
            <span>Payments</span>
            <span>Fintech UI</span>
            <span>Open Banking</span>
          </div>
        </div>

        <!-- TOOLS -->
        <div class="skill-card">
          <div class="skill-icon">
            ⚙
          </div>

          <h3>Tools & Workflow</h3>

          <p>
            Tools I use to write, manage, test and deploy my projects.
          </p>

          <div class="skill-tags">
            <span>Git</span>
            <span>GitHub</span>
            <span>VS Code</span>
            <span>npm</span>
            <span>Vercel</span>
            <span>Git Bash</span>
          </div>
        </div>

      </div>

    </div>
  </section>
</template>

<style scoped>
.skills-section {
  padding: 120px 7%;
  background: #050816;
}

.skills-container {
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
   SKILLS GRID
========================= */

.skills-grid {
  display: grid;

  grid-template-columns: repeat(2, 1fr);

  gap: 22px;
}

/* =========================
   SKILL CARD
========================= */

.skill-card {
  padding: 32px;

  min-height: 350px;

  border: 1px solid rgba(255, 255, 255, 0.07);

  border-radius: 20px;

  background: rgba(255, 255, 255, 0.025);

  transition: 0.3s ease;

  position: relative;

  overflow: hidden;
}

.skill-card::before {
  content: '';

  position: absolute;

  top: -100px;
  right: -100px;

  width: 200px;
  height: 200px;

  border-radius: 50%;

  background: rgba(37, 99, 235, 0.08);

  filter: blur(40px);

  transition: 0.3s ease;
}

.skill-card:hover {
  transform: translateY(-7px);

  border-color: rgba(59, 130, 246, 0.4);

  box-shadow:
    0 25px 60px rgba(0, 0, 0, 0.25);
}

.skill-card:hover::before {
  background: rgba(37, 99, 235, 0.16);
}

/* =========================
   ICON
========================= */

.skill-icon {
  width: 55px;
  height: 55px;

  display: flex;
  align-items: center;
  justify-content: center;

  border-radius: 14px;

  background: rgba(37, 99, 235, 0.1);

  border: 1px solid rgba(59, 130, 246, 0.2);

  color: #3b82f6;

  font-size: 22px;

  font-weight: 900;

  margin-bottom: 25px;
}

/* =========================
   TEXT
========================= */

.skill-card h3 {
  margin: 0;

  color: #ffffff;

  font-size: 21px;

  font-weight: 800;
}

.skill-card > p {
  margin-top: 12px;

  color: #94a3b8;

  font-size: 14px;

  line-height: 1.7;
}

/* =========================
   TAGS
========================= */

.skill-tags {
  display: flex;

  flex-wrap: wrap;

  gap: 9px;

  margin-top: 25px;
}

.skill-tags span {
  padding: 7px 11px;

  border-radius: 7px;

  background: rgba(255, 255, 255, 0.045);

  border: 1px solid rgba(255, 255, 255, 0.07);

  color: #cbd5e1;

  font-size: 12px;

  font-weight: 700;

  transition: 0.3s ease;
}

.skill-tags span:hover {
  color: #ffffff;

  border-color: rgba(59, 130, 246, 0.4);

  background: rgba(37, 99, 235, 0.1);
}

/* =========================
   TABLET
========================= */

@media (max-width: 850px) {
  .skills-grid {
    grid-template-columns: 1fr;
  }

  .skill-card {
    min-height: auto;
  }
}

/* =========================
   MOBILE
========================= */

@media (max-width: 550px) {
  .skills-section {
    padding: 90px 5%;
  }

  .skill-card {
    padding: 25px;
  }

  .skill-card h3 {
    font-size: 19px;
  }

  .section-heading h2 {
    font-size: 38px;
  }
}
</style>