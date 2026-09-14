<template>
  <footer class="footer">
    <div class="footer-container">

      <div class="footer-brand">
        <a href="#home" class="footer-logo">
          <span>M</span>ufasir
        </a>

        <p>
          Frontend Developer & Banking and Finance Student.
        </p>
      </div>

      <div class="footer-links">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
      </div>

      <div class="footer-bottom">
        <p>
          © 2026 Mufasir. All rights reserved.
        </p>

        <a href="#home">
          Back to top ↑
        </a>
      </div>

    </div>
  </footer>
</template>

<style scoped>
.footer {
  padding: 55px 7% 25px;
  background: #050816;
  border-top: 1px solid rgba(255, 255, 255, 0.06);
}

.footer-container {
  max-width: 1200px;
  margin: 0 auto;
}

/* BRAND */

.footer-brand {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 30px;
}

.footer-logo {
  color: #ffffff;
  text-decoration: none;

  font-size: 28px;
  font-weight: 900;
}

.footer-logo span {
  color: #3b82f6;
}

.footer-brand p {
  margin: 0;

  color: #64748b;

  font-size: 14px;
}

/* LINKS */

.footer-links {
  display: flex;
  gap: 28px;

  margin-top: 35px;
}

.footer-links a {
  color: #94a3b8;

  text-decoration: none;

  font-size: 13px;
  font-weight: 700;

  transition: 0.3s ease;
}

.footer-links a:hover {
  color: #3b82f6;
}

/* BOTTOM */

.footer-bottom {
  margin-top: 45px;
  padding-top: 22px;

  display: flex;
  justify-content: space-between;
  align-items: center;

  border-top: 1px solid rgba(255, 255, 255, 0.06);
}

.footer-bottom p {
  margin: 0;

  color: #475569;

  font-size: 12px;
}

.footer-bottom a {
  color: #64748b;

  text-decoration: none;

  font-size: 12px;
  font-weight: 700;

  transition: 0.3s ease;
}

.footer-bottom a:hover {
  color: #3b82f6;
}

/* RESPONSIVE */

@media (max-width: 650px) {
  .footer {
    padding: 45px 5% 22px;
  }

  .footer-brand {
    align-items: flex-start;
    flex-direction: column;
  }

  .footer-links {
    flex-wrap: wrap;
    gap: 18px;
  }

  .footer-bottom {
    align-items: flex-start;
    flex-direction: column;
    gap: 15px;
  }
}
</style>