<template>
  <section id="contact" class="contact-section">
    <div class="contact-container">

      <div class="contact-heading">
        <span>GET IN TOUCH</span>

        <h2>
          Let's build something
          <strong>great together.</strong>
        </h2>

        <p>
          Have a project, opportunity or idea you'd like to discuss?
          I'd love to hear from you.
        </p>
      </div>

      <div class="contact-grid">

        <!-- CONTACT INFO -->
        <div class="contact-info">

          <a
            href="mailto:mufasirdevmaster@gmail.com"
            class="contact-card"
          >
            <div class="contact-icon">
              @
            </div>

            <div>
              <span>Email</span>
              <strong>muhsinadebayo366@gmail.com</strong>
            </div>

            <span class="arrow">↗</span>
          </a>

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
              <strong>Let's chat on WhatsApp</strong>
            </div>

            <span class="arrow">↗</span>
          </a>

          <div class="contact-card">
            <div class="contact-icon">
              N
            </div>

            <div>
              <span>Based in</span>
              <strong>Nigeria</strong>
            </div>
          </div>

        </div>

        <!-- MESSAGE CARD -->
        <div class="message-card">
          <div class="message-number">01</div>

          <h3>Have an idea?</h3>

          <p>
            Whether it's a website, financial technology project,
            collaboration or something completely new, let's talk
            about it.
          </p>

          <a
            href="mailto:mufasirdevmaster@gmail.com"
            class="message-button"
          >
            Send Me a Message
            <span>→</span>
          </a>
        </div>

      </div>

    </div>
  </section>
</template>

<style scoped>
.contact-section {
  padding: 130px 7%;
  background: #070d1f;
}

.contact-container {
  max-width: 1200px;
  margin: 0 auto;
}

/* HEADING */

.contact-heading {
  max-width: 800px;
  margin-bottom: 65px;
}

.contact-heading > span {
  color: #3b82f6;

  font-size: 13px;
  font-weight: 800;
  letter-spacing: 3px;
}

.contact-heading h2 {
  margin: 15px 0 20px;

  color: #ffffff;

  font-size: clamp(40px, 5.5vw, 68px);
  line-height: 1.05;
  font-weight: 900;
}

.contact-heading h2 strong {
  display: block;
  color: #3b82f6;
}

.contact-heading p {
  max-width: 650px;

  color: #94a3b8;

  font-size: 16px;
  line-height: 1.8;
}

/* GRID */

.contact-grid {
  display: grid;
  grid-template-columns: 1fr 0.9fr;
  gap: 25px;
}

/* CONTACT INFO */

.contact-info {
  display: flex;
  flex-direction: column;
  gap: 15px;
}

.contact-card {
  min-height: 95px;
  padding: 20px 22px;

  display: flex;
  align-items: center;
  gap: 17px;

  position: relative;

  border: 1px solid rgba(255, 255, 255, 0.07);
  border-radius: 15px;

  background: rgba(255, 255, 255, 0.025);

  text-decoration: none;

  transition: 0.3s ease;
}

a.contact-card:hover {
  transform: translateX(5px);

  border-color: rgba(59, 130, 246, 0.4);

  background: rgba(37, 99, 235, 0.05);
}

.contact-icon {
  width: 50px;
  height: 50px;

  flex-shrink: 0;

  display: flex;
  align-items: center;
  justify-content: center;

  border-radius: 12px;

  color: #3b82f6;
  background: rgba(37, 99, 235, 0.1);

  font-size: 18px;
  font-weight: 900;
}

.contact-card div:nth-child(2) {
  display: flex;
  flex-direction: column;
  gap: 5px;
}

.contact-card span:not(.arrow) {
  color: #64748b;

  font-size: 11px;
  font-weight: 800;
  letter-spacing: 1px;
  text-transform: uppercase;
}

.contact-card strong {
  color: #e2e8f0;

  font-size: 14px;
  font-weight: 700;
}

.arrow {
  margin-left: auto;

  color: #3b82f6;

  font-size: 20px;
}

/* MESSAGE CARD */

.message-card {
  position: relative;

  min-height: 300px;
  padding: 40px;

  overflow: hidden;

  display: flex;
  flex-direction: column;
  justify-content: center;

  border: 1px solid rgba(59, 130, 246, 0.2);
  border-radius: 20px;

  background:
    linear-gradient(
      145deg,
      rgba(37, 99, 235, 0.15),
      rgba(255, 255, 255, 0.025)
    );
}

.message-card::after {
  content: "";

  position: absolute;

  width: 220px;
  height: 220px;

  right: -100px;
  bottom: -100px;

  border-radius: 50%;

  background: rgba(37, 99, 235, 0.12);

  filter: blur(10px);
}

.message-number {
  position: absolute;

  top: 25px;
  right: 30px;

  color: rgba(59, 130, 246, 0.5);

  font-size: 12px;
  font-weight: 900;
}

.message-card h3 {
  margin: 0 0 15px;

  color: #ffffff;

  font-size: 30px;
  font-weight: 900;
}

.message-card p {
  max-width: 470px;

  color: #94a3b8;

  font-size: 15px;
  line-height: 1.8;
}

.message-button {
  width: fit-content;

  margin-top: 25px;
  padding: 14px 20px;

  display: inline-flex;
  align-items: center;
  gap: 12px;

  color: #ffffff;
  background: #2563eb;

  border-radius: 9px;

  text-decoration: none;

  font-size: 13px;
  font-weight: 800;

  transition: 0.3s ease;
}

.message-button:hover {
  background: #1d4ed8;
  transform: translateY(-3px);
}

.message-button span {
  font-size: 18px;
}

/* RESPONSIVE */

@media (max-width: 850px) {
  .contact-grid {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 600px) {
  .contact-section {
    padding: 90px 5%;
  }

  .contact-card {
    padding: 17px;
  }

  .contact-card strong {
    font-size: 13px;
  }

  .message-card {
    padding: 30px;
  }
}
</style>