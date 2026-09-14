<template>
  <section id="experience" class="experience-section">
    <div class="experience-container">

      <div class="section-heading">
        <span>MY EXPERIENCE</span>
        <h2>Where technology meets finance.</h2>
      </div>

      <div class="experience-list">

        <!-- EXPERIENCE 1 -->
        <div class="experience-card">
          <div class="experience-year">
            <span>01</span>
            <div></div>
          </div>

          <div class="experience-content">
            <div class="experience-top">
              <div>
                <span class="experience-type">
                  Technology
                </span>

                <h3>Frontend Development</h3>
              </div>

              <span class="experience-date">
                2024 — Present
              </span>
            </div>

            <p>
              Developing modern web interfaces and applications using
              technologies such as HTML, CSS, JavaScript, Vue.js and Vite.
              I focus on responsive design, clean user interfaces and
              practical digital solutions.
            </p>

            <div class="experience-tags">
              <span>HTML</span>
              <span>CSS</span>
              <span>JavaScript</span>
              <span>Vue.js</span>
              <span>Vite</span>
              <span>Git</span>
            </div>
          </div>
        </div>

        <!-- EXPERIENCE 2 -->
        <div class="experience-card">
          <div class="experience-year">
            <span>02</span>
            <div></div>
          </div>

          <div class="experience-content">
            <div class="experience-top">
              <div>
                <span class="experience-type">
                  Finance
                </span>

                <h3>Banking & Finance</h3>
              </div>

              <span class="experience-date">
                2025 — Present
              </span>
            </div>

            <p>
              Studying Banking and Finance while developing an interest
              in digital banking, fintech, open banking and financial
              technology. I enjoy combining financial knowledge with
              technology to build useful solutions.
            </p>

            <div class="experience-tags">
              <span>Banking</span>
              <span>Finance</span>
              <span>Fintech</span>
              <span>Open Banking</span>
            </div>
          </div>
        </div>

        <!-- EXPERIENCE 3 -->
        <div class="experience-card">
          <div class="experience-year">
            <span>03</span>
            <div></div>
          </div>

          <div class="experience-content">
            <div class="experience-top">
              <div>
                <span class="experience-type">
                  Leadership
                </span>

                <h3>Student Leadership</h3>
              </div>

              <span class="experience-date">
                University
              </span>
            </div>

            <p>
              Building leadership, communication and teamwork skills
              through student activities and responsibilities within
              the university community.
            </p>

            <div class="experience-tags">
              <span>Leadership</span>
              <span>Communication</span>
              <span>Teamwork</span>
              <span>Organization</span>
            </div>
          </div>
        </div>

      </div>

    </div>
  </section>
</template>

<style scoped>
.experience-section {
  padding: 120px 7%;
  background: #050816;
}

.experience-container {
  max-width: 1100px;
  margin: 0 auto;
}

/* HEADING */

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

/* EXPERIENCE LIST */

.experience-list {
  display: flex;
  flex-direction: column;
  gap: 22px;
}

.experience-card {
  display: grid;
  grid-template-columns: 80px 1fr;
  gap: 25px;

  padding: 32px;

  border: 1px solid rgba(255, 255, 255, 0.07);
  border-radius: 18px;

  background: rgba(255, 255, 255, 0.025);

  transition: 0.35s ease;
}

.experience-card:hover {
  transform: translateX(6px);

  border-color: rgba(59, 130, 246, 0.35);

  background: rgba(37, 99, 235, 0.035);
}

/* NUMBER */

.experience-year {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.experience-year span {
  width: 48px;
  height: 48px;

  display: flex;
  align-items: center;
  justify-content: center;

  border-radius: 12px;

  color: #3b82f6;
  background: rgba(37, 99, 235, 0.1);

  font-size: 13px;
  font-weight: 900;
}

.experience-year div {
  width: 1px;
  flex: 1;

  margin-top: 15px;

  background: rgba(59, 130, 246, 0.15);
}

/* CONTENT */

.experience-content {
  min-width: 0;
}

.experience-top {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  gap: 20px;
}

.experience-type {
  color: #3b82f6;

  font-size: 11px;
  font-weight: 800;
  letter-spacing: 1.5px;
  text-transform: uppercase;
}

.experience-content h3 {
  margin: 8px 0 15px;

  color: #ffffff;

  font-size: 25px;
  font-weight: 900;
}

.experience-date {
  color: #64748b;

  font-size: 12px;
  font-weight: 700;

  white-space: nowrap;
}

.experience-content p {
  max-width: 850px;

  color: #94a3b8;

  font-size: 15px;
  line-height: 1.8;
}

/* TAGS */

.experience-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;

  margin-top: 22px;
}

.experience-tags span {
  padding: 7px 11px;

  border-radius: 6px;

  color: #cbd5e1;
  background: rgba(255, 255, 255, 0.05);

  font-size: 11px;
  font-weight: 700;
}

/* RESPONSIVE */

@media (max-width: 700px) {
  .experience-section {
    padding: 90px 5%;
  }

  .experience-card {
    grid-template-columns: 1fr;
    gap: 20px;
    padding: 25px;
  }

  .experience-year {
    flex-direction: row;
    justify-content: flex-start;
  }

  .experience-year div {
    display: none;
  }

  .experience-top {
    flex-direction: column;
    gap: 5px;
  }

  .experience-date {
    white-space: normal;
  }
}
</style>