<template>
  <section id="about" class="about-section">
    <div class="about-container">

      <div class="section-heading">
        <span>ABOUT ME</span>
        <h2>Turning ideas into digital experiences.</h2>
      </div>

      <div class="about-grid">

        <div class="about-content">
          <p class="intro">
            I'm <strong>Adebayo Muh'sin Adebola</strong>, a Banking and
            Finance student and Frontend Developer passionate about
            technology, creativity and building useful digital products.
          </p>

          <p>
            My journey combines two different worlds — finance and
            technology. I enjoy using modern web technologies to turn
            ideas into clean, responsive and user-friendly applications.
          </p>

          <p>
            I'm continuously improving my skills in frontend development,
            exploring new technologies and working on projects that solve
            real-world problems.
          </p>

          <a href="#contact" class="about-button">
            Let's Work Together
          </a>
        </div>

        <div class="about-stats">

          <div class="stat-card">
            <strong>03+</strong>
            <span>Projects Built</span>
          </div>

          <div class="stat-card">
            <strong>02+</strong>
            <span>Years Learning Tech</span>
          </div>

          <div class="stat-card">
            <strong>01</strong>
            <span>Developer Journey</span>
          </div>

          <div class="stat-card">
            <strong>100%</strong>
            <span>Passion for Growth</span>
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

/* SECTION HEADING */

.section-heading {
  max-width: 750px;
  margin-bottom: 65px;
}

.section-heading span {
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
}

/* CONTENT */

.about-grid {
  display: grid;
  grid-template-columns: 1.1fr 0.9fr;
  gap: 80px;
  align-items: center;
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

/* BUTTON */

.about-button {
  display: inline-block;
  margin-top: 15px;
  padding: 14px 23px;

  color: #ffffff;
  background: #2563eb;

  text-decoration: none;
  font-weight: 800;
  border-radius: 9px;

  transition: 0.3s ease;
}

.about-button:hover {
  background: #1d4ed8;
  transform: translateY(-3px);
}

/* STATS */

.about-stats {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 18px;
}

.stat-card {
  min-height: 170px;
  padding: 30px;

  display: flex;
  flex-direction: column;
  justify-content: center;

  border: 1px solid rgba(255, 255, 255, 0.07);
  border-radius: 18px;

  background: rgba(255, 255, 255, 0.025);

  transition: 0.3s ease;
}

.stat-card:hover {
  transform: translateY(-6px);
  border-color: rgba(59, 130, 246, 0.4);
  background: rgba(37, 99, 235, 0.06);
}

.stat-card strong {
  color: #3b82f6;
  font-size: 38px;
  font-weight: 900;
}

.stat-card span {
  margin-top: 8px;
  color: #94a3b8;
  font-size: 14px;
  font-weight: 600;
}

/* RESPONSIVE */

@media (max-width: 900px) {
  .about-grid {
    grid-template-columns: 1fr;
    gap: 50px;
  }

  .about-content {
    max-width: 750px;
  }
}

@media (max-width: 550px) {
  .about-section {
    padding: 90px 5%;
  }

  .about-stats {
    grid-template-columns: 1fr;
  }

  .stat-card {
    min-height: 140px;
  }
}
</style>