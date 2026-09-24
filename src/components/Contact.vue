<template>
  <section id="contact" class="contact-section">
    <div class="contact-container">

      <!-- HEADER -->
      <div class="section-heading">
        <span>GET IN TOUCH</span>

        <h2>
          Let's build something
          <span>great together.</span>
        </h2>

        <p>
          Have a project, business idea or opportunity you'd like
          to discuss? Feel free to reach out.
        </p>
      </div>

      <!-- CONTACT GRID -->
      <div class="contact-grid">

        <!-- CONTACT INFO -->
        <div class="contact-info">

          <!-- EMAIL -->
          <a
            href="mailto:mufasirdevmaster@gmail.com"
            class="contact-card"
          >
            <div class="contact-icon">
              @
            </div>

            <div>
              <span>Email</span>
              <h3>mufasirdevmaster@gmail.com</h3>
            </div>

            <strong>↗</strong>
          </a>

          <!-- WHATSAPP -->
          <a
            href="https://wa.me/2348093963715"
            target="_blank"
            rel="noopener noreferrer"
            class="contact-card"
          >
            <div class="contact-icon">
              W
            </div>

            <div>
              <span>WhatsApp</span>
              <h3>Let's chat on WhatsApp</h3>
            </div>

            <strong>↗</strong>
          </a>

          <!-- LOCATION -->
          <div class="contact-card location-card">
            <div class="contact-icon">
              N
            </div>

            <div>
              <span>Based in</span>
              <h3>Nigeria</h3>
            </div>
          </div>

        </div>

        <!-- RIGHT CARD -->
        <div class="contact-cta">

          <div class="cta-number">
            01
          </div>

          <h3>
            Have an idea?
          </h3>

          <p>
            Whether you need a website, web application, fintech
            interface or a digital product, I'd love to hear about it.
          </p>

          <a
            href="mailto:mufasirdevmaster@gmail.com?subject=Project%20Inquiry"
            class="contact-button"
          >
            Start a Conversation
            <span>↗</span>
          </a>

        </div>

      </div>

    </div>
  </section>
</template>

<style scoped>
.contact-section {
  padding: 120px 7%;
  background: #070d1f;
}

.contact-container {
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
  max-width: 650px;

  margin-top: 20px;

  color: #94a3b8;

  font-size: 16px;
  line-height: 1.8;
}

/* =========================
   CONTACT GRID
========================= */

.contact-grid {
  display: grid;

  grid-template-columns: 1fr 0.85fr;

  gap: 25px;

  align-items: stretch;
}

/* =========================
   CONTACT INFO
========================= */

.contact-info {
  display: flex;

  flex-direction: column;

  gap: 15px;
}

/* =========================
   CONTACT CARD
========================= */

.contact-card {
  min-height: 105px;

  padding: 22px 25px;

  display: flex;

  align-items: center;

  gap: 18px;

  text-decoration: none;

  border: 1px solid rgba(255, 255, 255, 0.07);

  border-radius: 16px;

  background: rgba(255, 255, 255, 0.025);

  transition: 0.3s ease;
}

.contact-card:hover {
  transform: translateX(6px);

  border-color: rgba(59, 130, 246, 0.4);

  background: rgba(37, 99, 235, 0.06);
}

/* =========================
   ICON
========================= */

.contact-icon {
  width: 50px;
  height: 50px;

  flex-shrink: 0;

  display: flex;

  align-items: center;
  justify-content: center;

  border-radius: 13px;

  color: #3b82f6;

  background: rgba(37, 99, 235, 0.1);

  border: 1px solid rgba(59, 130, 246, 0.18);

  font-size: 19px;

  font-weight: 900;
}

/* =========================
   CARD TEXT
========================= */

.contact-card div:nth-child(2) {
  flex: 1;
}

.contact-card span {
  display: block;

  color: #64748b;

  font-size: 11px;

  font-weight: 800;

  letter-spacing: 1.5px;

  text-transform: uppercase;
}

.contact-card h3 {
  margin-top: 6px;

  color: #e2e8f0;

  font-size: 15px;

  font-weight: 700;

  word-break: break-word;
}

.contact-card > strong {
  color: #3b82f6;

  font-size: 19px;

  transition: 0.3s ease;
}

.contact-card:hover > strong {
  transform: translate(3px, -3px);
}

/* LOCATION */

.location-card {
  cursor: default;
}

.location-card:hover {
  transform: none;
}

/* =========================
   CTA CARD
========================= */

.contact-cta {
  padding: 40px;

  min-height: 100%;

  display: flex;

  flex-direction: column;

  justify-content: center;

  border-radius: 20px;

  border: 1px solid rgba(59, 130, 246, 0.2);

  background:
    linear-gradient(
      145deg,
      rgba(37, 99, 235, 0.12),
      rgba(255, 255, 255, 0.025)
    );

  position: relative;

  overflow: hidden;
}

.contact-cta::before {
  content: '';

  position: absolute;

  width: 250px;
  height: 250px;

  right: -100px;
  bottom: -130px;

  border-radius: 50%;

  background: rgba(37, 99, 235, 0.15);

  filter: blur(40px);
}

/* =========================
   CTA CONTENT
========================= */

.cta-number {
  color: #3b82f6;

  font-size: 12px;

  font-weight: 900;

  letter-spacing: 2px;
}

.contact-cta h3 {
  margin-top: 20px;

  color: #ffffff;

  font-size: 34px;

  font-weight: 900;

  position: relative;
}

.contact-cta p {
  max-width: 450px;

  margin-top: 15px;

  color: #94a3b8;

  font-size: 15px;

  line-height: 1.8;

  position: relative;
}

/* =========================
   CTA BUTTON
========================= */

.contact-button {
  width: fit-content;

  display: inline-flex;

  align-items: center;

  gap: 10px;

  margin-top: 30px;

  padding: 14px 20px;

  color: #ffffff;

  background: #2563eb;

  border-radius: 9px;

  text-decoration: none;

  font-size: 14px;

  font-weight: 800;

  position: relative;

  transition: 0.3s ease;
}

.contact-button:hover {
  background: #1d4ed8;

  transform: translateY(-3px);
}

.contact-button span {
  font-size: 18px;

  transition: 0.3s ease;
}

.contact-button:hover span {
  transform: translate(3px, -3px);
}

/* =========================
   TABLET
========================= */

@media (max-width: 850px) {
  .contact-grid {
    grid-template-columns: 1fr;
  }

  .contact-cta {
    min-height: 320px;
  }
}

/* =========================
   MOBILE
========================= */

@media (max-width: 550px) {
  .contact-section {
    padding: 90px 5%;
  }

  .contact-card {
    padding: 18px;

    gap: 13px;
  }

  .contact-icon {
    width: 45px;
    height: 45px;
  }

  .contact-card h3 {
    font-size: 13px;
  }

  .contact-cta {
    padding: 28px;

    min-height: 300px;
  }

  .contact-cta h3 {
    font-size: 29px;
  }

  .contact-button {
    width: 100%;

    justify-content: center;

    text-align: center;
  }
}
</style>