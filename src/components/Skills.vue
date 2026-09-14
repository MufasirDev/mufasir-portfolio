<template>
  <section id="skills" class="skills-section">
    <div class="skills-container">

      <div class="section-heading">
        <span>MY SKILLS</span>
        <h2>Tools I use to bring ideas to life.</h2>
      </div>

      <div class="skills-grid">

        <div class="skill-card">
          <div class="skill-number">01</div>
          <div class="skill-icon">&lt;/&gt;</div>
          <h3>HTML</h3>
          <p>
            Building clean and well-structured web pages using modern
            HTML standards.
          </p>
        </div>

        <div class="skill-card">
          <div class="skill-number">02</div>
          <div class="skill-icon">#</div>
          <h3>CSS</h3>
          <p>
            Creating responsive layouts, animations and modern visual
            experiences.
          </p>
        </div>

        <div class="skill-card">
          <div class="skill-number">03</div>
          <div class="skill-icon">JS</div>
          <h3>JavaScript</h3>
          <p>
            Adding functionality and interactive features to modern
            web applications.
          </p>
        </div>

        <div class="skill-card">
          <div class="skill-number">04</div>
          <div class="skill-icon">V</div>
          <h3>Vue.js</h3>
          <p>
            Developing scalable and interactive interfaces with Vue.js.
          </p>
        </div>

        <div class="skill-card">
          <div class="skill-number">05</div>
          <div class="skill-icon">⚡</div>
          <h3>Vite</h3>
          <p>
            Using Vite to build fast and modern frontend applications.
          </p>
        </div>

        <div class="skill-card">
          <div class="skill-number">06</div>
          <div class="skill-icon">G</div>
          <h3>Git & GitHub</h3>
          <p>
            Managing projects, tracking changes and collaborating
            through Git and GitHub.
          </p>
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

.section-heading {
  max-width: 750px;
  margin-bottom: 60px;
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

/* GRID */

.skills-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

.skill-card {
  position: relative;
  min-height: 270px;
  padding: 32px;

  overflow: hidden;

  border: 1px solid rgba(255, 255, 255, 0.07);
  border-radius: 18px;

  background: rgba(255, 255, 255, 0.025);

  transition: 0.35s ease;
}

.skill-card::before {
  content: "";
  position: absolute;
  width: 120px;
  height: 120px;
  top: -60px;
  right: -60px;

  border-radius: 50%;
  background: rgba(37, 99, 235, 0.12);
}

.skill-card:hover {
  transform: translateY(-8px);
  border-color: rgba(59, 130, 246, 0.45);
  background: rgba(37, 99, 235, 0.05);
  box-shadow: 0 20px 50px rgba(0, 0, 0, 0.2);
}

.skill-number {
  position: absolute;
  top: 25px;
  right: 28px;

  color: #334155;
  font-size: 12px;
  font-weight: 900;
}

.skill-icon {
  width: 55px;
  height: 55px;

  display: flex;
  align-items: center;
  justify-content: center;

  margin-bottom: 25px;

  border-radius: 13px;

  color: #3b82f6;
  background: rgba(37, 99, 235, 0.1);

  font-size: 20px;
  font-weight: 900;
}

.skill-card h3 {
  margin: 0 0 12px;

  color: #ffffff;
  font-size: 21px;
  font-weight: 800;
}

.skill-card p {
  margin: 0;

  color: #94a3b8;
  font-size: 14px;
  line-height: 1.7;
}

/* RESPONSIVE */

@media (max-width: 950px) {
  .skills-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 600px) {
  .skills-section {
    padding: 90px 5%;
  }

  .skills-grid {
    grid-template-columns: 1fr;
  }

  .skill-card {
    min-height: 240px;
  }
}
</style>