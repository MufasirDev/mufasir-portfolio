<template>
  <section id="experience" class="experience-section">
    <div class="experience-container">

      <!-- SECTION HEADER -->
      <div class="section-heading">
        <span>MY JOURNEY</span>

        <h2>
          Where my journey meets
          <span>technology.</span>
        </h2>

        <p>
          A combination of education, technology, entrepreneurship and
          hands-on project building that continues to shape my career.
        </p>
      </div>

      <!-- TIMELINE -->
      <div class="timeline">

        <!-- ITEM 1 -->
        <div class="timeline-item">

          <div class="timeline-marker">
            <span>01</span>
          </div>

          <div class="timeline-content">

            <div class="timeline-top">
              <div>
                <span class="timeline-type">
                  TECHNOLOGY
                </span>

                <h3>
                  Frontend Developer & Product Builder
                </h3>
              </div>

              <span class="timeline-date">
                Present
              </span>
            </div>

            <p>
              Building modern websites and web applications using
              technologies such as HTML, CSS, JavaScript, Vue.js and
              Vite. I focus on responsive interfaces, clean user
              experiences and practical digital solutions.
            </p>

            <div class="timeline-tags">
              <span>Vue.js</span>
              <span>JavaScript</span>
              <span>Vite</span>
              <span>Responsive Design</span>
            </div>

          </div>

        </div>

        <!-- ITEM 2 -->
        <div class="timeline-item">

          <div class="timeline-marker">
            <span>02</span>
          </div>

          <div class="timeline-content">

            <div class="timeline-top">
              <div>
                <span class="timeline-type">
                  ENTREPRENEURSHIP
                </span>

                <h3>
                  Mufasir Tech / Devmaster Academy
                </h3>
              </div>

              <span class="timeline-date">
                Present
              </span>
            </div>

            <p>
              Building digital products and creating technology-focused
              learning experiences through Mufasir Tech and Mufasir
              Devmaster Academy. The work combines development,
              education and digital entrepreneurship.
            </p>

            <div class="timeline-tags">
              <span>Web Development</span>
              <span>Education</span>
              <span>Product Building</span>
              <span>Digital Business</span>
            </div>

          </div>

        </div>

        <!-- ITEM 3 -->
        <div class="timeline-item">

          <div class="timeline-marker">
            <span>03</span>
          </div>

          <div class="timeline-content">

            <div class="timeline-top">
              <div>
                <span class="timeline-type">
                  FINTECH
                </span>

                <h3>
                  Fintech & Digital Finance Projects
                </h3>
              </div>

              <span class="timeline-date">
                Ongoing
              </span>
            </div>

            <p>
              Exploring the intersection between finance and
              technology through projects such as MufasirPay,
              FinView and BankScope. My focus includes digital
              wallets, payments, financial dashboards and open
              banking concepts.
            </p>

            <div class="timeline-tags">
              <span>Fintech</span>
              <span>Digital Wallets</span>
              <span>Payments</span>
              <span>Open Banking</span>
            </div>

          </div>

        </div>

        <!-- ITEM 4 -->
        <div class="timeline-item">

          <div class="timeline-marker">
            <span>04</span>
          </div>

          <div class="timeline-content">

            <div class="timeline-top">
              <div>
                <span class="timeline-type">
                  EDUCATION
                </span>

                <h3>
                  Banking & Finance — University of Abuja
                </h3>
              </div>

              <span class="timeline-date">
                300 Level
              </span>
            </div>

            <p>
              Studying Banking and Finance while developing a strong
              interest in financial technology, digital banking and
              the role of technology in modern financial services.
            </p>

            <div class="timeline-tags">
              <span>Banking</span>
              <span>Finance</span>
              <span>Financial Technology</span>
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

/* =========================
   SECTION HEADER
========================= */

.section-heading {
  max-width: 850px;
  margin-bottom: 70px;
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
   TIMELINE
========================= */

.timeline {
  position: relative;
}

/* vertical line */

.timeline::before {
  content: '';

  position: absolute;

  top: 0;
  bottom: 0;

  left: 27px;

  width: 1px;

  background:
    linear-gradient(
      to bottom,
      rgba(59, 130, 246, 0.6),
      rgba(59, 130, 246, 0.08)
    );
}

/* =========================
   TIMELINE ITEM
========================= */

.timeline-item {
  position: relative;

  display: grid;

  grid-template-columns: 55px 1fr;

  gap: 30px;

  margin-bottom: 35px;
}

.timeline-item:last-child {
  margin-bottom: 0;
}

/* =========================
   MARKER
========================= */

.timeline-marker {
  width: 55px;
  height: 55px;

  display: flex;

  align-items: center;
  justify-content: center;

  border-radius: 50%;

  background: #07112b;

  border: 1px solid rgba(59, 130, 246, 0.45);

  box-shadow:
    0 0 0 7px #050816;

  z-index: 2;
}

.timeline-marker span {
  color: #3b82f6;

  font-size: 12px;

  font-weight: 900;
}

/* =========================
   CONTENT
========================= */

.timeline-content {
  padding: 30px;

  border: 1px solid rgba(255, 255, 255, 0.07);

  border-radius: 18px;

  background: rgba(255, 255, 255, 0.025);

  transition: 0.3s ease;
}

.timeline-content:hover {
  transform: translateX(5px);

  border-color: rgba(59, 130, 246, 0.35);

  background: rgba(37, 99, 235, 0.045);

  box-shadow:
    0 20px 50px rgba(0, 0, 0, 0.2);
}

/* =========================
   TOP
========================= */

.timeline-top {
  display: flex;

  justify-content: space-between;

  align-items: flex-start;

  gap: 20px;
}

.timeline-type {
  color: #3b82f6;

  font-size: 11px;

  font-weight: 900;

  letter-spacing: 2px;
}

.timeline-content h3 {
  margin-top: 8px;

  color: #ffffff;

  font-size: 22px;

  font-weight: 900;

  line-height: 1.3;
}

.timeline-date {
  flex-shrink: 0;

  padding: 7px 11px;

  border-radius: 7px;

  color: #94a3b8;

  background: rgba(255, 255, 255, 0.04);

  border: 1px solid rgba(255, 255, 255, 0.07);

  font-size: 11px;

  font-weight: 700;
}

/* =========================
   DESCRIPTION
========================= */

.timeline-content > p {
  margin-top: 18px;

  color: #94a3b8;

  font-size: 14px;

  line-height: 1.8;
}

/* =========================
   TAGS
========================= */

.timeline-tags {
  display: flex;

  flex-wrap: wrap;

  gap: 8px;

  margin-top: 22px;
}

.timeline-tags span {
  padding: 7px 10px;

  border-radius: 6px;

  color: #cbd5e1;

  background: rgba(255, 255, 255, 0.04);

  border: 1px solid rgba(255, 255, 255, 0.06);

  font-size: 11px;

  font-weight: 700;
}

/* =========================
   TABLET
========================= */

@media (max-width: 700px) {
  .timeline-item {
    grid-template-columns: 45px 1fr;

    gap: 18px;
  }

  .timeline::before {
    left: 22px;
  }

  .timeline-marker {
    width: 45px;
    height: 45px;
  }

  .timeline-content {
    padding: 24px;
  }

  .timeline-top {
    flex-direction: column;
    gap: 12px;
  }
}

/* =========================
   MOBILE
========================= */

@media (max-width: 550px) {
  .experience-section {
    padding: 90px 5%;
  }

  .timeline-item {
    grid-template-columns: 1fr;

    gap: 15px;
  }

  .timeline::before {
    display: none;
  }

  .timeline-marker {
    width: 42px;
    height: 42px;

    box-shadow: none;
  }

  .timeline-content {
    padding: 22px;
  }

  .timeline-content h3 {
    font-size: 19px;
  }

  .timeline-date {
    align-self: flex-start;
  }
}
</style>