<template>
  <section id="about" class="about-section">
    <div class="about-container">

      <!-- SECTION HEADER -->
      <div class="section-heading">
        <span>ABOUT ME</span>

        <h2>
          Technology, finance and creativity —
          <span>all in one journey.</span>
        </h2>
      </div>

      <!-- CONTENT -->
      <div class="about-grid">

        <!-- LEFT -->
        <div class="about-content">

          <p class="intro">
            I'm <strong>Adebayo Muh'sin Adebola</strong>, a Frontend
            Developer and Banking & Finance student passionate about
            building modern digital products.
          </p>

          <p>
            I enjoy transforming ideas into responsive, user-friendly
            websites and applications. My work focuses on creating
            interfaces that are not only visually appealing but also
            practical and easy to use.
          </p>

          <p>
            My background in Banking and Finance has also influenced
            my interest in fintech, financial technology and digital
            financial solutions. I enjoy exploring how technology can
            improve the way people interact with financial services.
          </p>

          <p>
            I'm currently developing projects across frontend
            development, fintech and digital platforms while
            continuously improving my technical and problem-solving
            skills.
          </p>

          <div class="about-buttons">
            <a href="#projects" class="about-button primary">
              Explore My Projects
            </a>

            <a href="#contact" class="about-button secondary">
              Let's Connect
            </a>
          </div>

        </div>

        <!-- RIGHT -->
        <div class="about-stats">

          <div class="stat-card">
            <div class="stat-number">01</div>

            <div>
              <h3>Frontend Developer</h3>
              <p>
                Building responsive and modern web experiences.
              </p>
            </div>
          </div>

          <div class="stat-card">
            <div class="stat-number">02</div>

            <div>
              <h3>Fintech Builder</h3>
              <p>
                Exploring digital finance and financial technology.
              </p>
            </div>
          </div>

          <div class="stat-card">
            <div class="stat-number">03</div>

            <div>
              <h3>Banking & Finance</h3>
              <p>
                Studying finance while connecting it with technology.
              </p>
            </div>
          </div>

          <div class="stat-card">
            <div class="stat-number">04</div>

            <div>
              <h3>Continuous Growth</h3>
              <p>
                Learning, building and improving every day.
              </p>
            </div>
          </div>

        </div>

      </div>

    </div>
  </section>
</template>

<style scoped>
.about-section {
  padding: 120px 7%;
  background: #070d1f;
}

.about-container {
  max-width: 1200px;
  margin: 0 auto;
}

/* =========================
   SECTION HEADING
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

/* =========================
   GRID
========================= */

.about-grid {
  display: grid;
  grid-template-columns: 1.1fr 0.9fr;
  gap: 80px;
  align-items: center;
}

/* =========================
   CONTENT
========================= */

.about-content {
  max-width: 700px;
}

.about-content p {
  color: #94a3b8;
  font-size: 16px;
  line-height: 1.9;
  margin-bottom: 22px;
}

.about-content .intro {
  color: #cbd5e1;
  font-size: 20px;
  line-height: 1.7;
}

.about-content strong {
  color: #ffffff;
}

/* =========================
   BUTTONS
========================= */

.about-buttons {
  display: flex;
  gap: 14px;
  flex-wrap: wrap;
  margin-top: 30px;
}

.about-button {
  display: inline-block;
  padding: 14px 21px;

  text-decoration: none;
  font-weight: 800;

  border-radius: 9px;

  transition: 0.3s ease;
}

.about-button.primary {
  color: #ffffff;
  background: #2563eb;
}

.about-button.primary:hover {
  background: #1d4ed8;
  transform: translateY(-3px);
}

.about-button.secondary {
  color: #ffffff;
  border: 1px solid rgba(255, 255, 255, 0.14);
  background: rgba(255, 255, 255, 0.03);
}

.about-button.secondary:hover {
  border-color: #3b82f6;
  transform: translateY(-3px);
}

/* =========================
   STAT CARDS
========================= */

.about-stats {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 18px;
}

.stat-card {
  min-height: 190px;
  padding: 28px;

  display: flex;
  flex-direction: column;
  justify-content: space-between;

  border: 1px solid rgba(255, 255, 255, 0.07);
  border-radius: 18px;

  background: rgba(255, 255, 255, 0.025);

  transition: 0.3s ease;
}

.stat-card:hover {
  transform: translateY(-6px);

  border-color: rgba(59, 130, 246, 0.4);

  background: rgba(37, 99, 235, 0.06);

  box-shadow:
    0 20px 45px rgba(0, 0, 0, 0.2);
}

.stat-number {
  color: #3b82f6;
  font-size: 14px;
  font-weight: 900;
  letter-spacing: 2px;
}

.stat-card h3 {
  margin: 15px 0 8px;

  color: #ffffff;
  font-size: 18px;
  font-weight: 800;
}

.stat-card p {
  margin: 0;

  color: #64748b;
  font-size: 13px;
  line-height: 1.6;
}

/* =========================
   TABLET
========================= */

@media (max-width: 900px) {
  .about-grid {
    grid-template-columns: 1fr;
    gap: 55px;
  }

  .about-content {
    max-width: 750px;
  }
}

/* =========================
   MOBILE
========================= */

@media (max-width: 550px) {
  .about-section {
    padding: 90px 5%;
  }

  .about-stats {
    grid-template-columns: 1fr;
  }

  .stat-card {
    min-height: 160px;
  }

  .about-buttons {
    flex-direction: column;
  }

  .about-button {
    text-align: center;
  }
}
</style>