<template>
  <footer class="footer">

    <div class="footer-container">

      <!-- BRAND -->
      <div class="footer-brand">

        <a href="#home" class="footer-logo">
          <span>M</span>ufasir
          <span>D</span>ev
        </a>

        <p>
          Frontend Developer • Fintech Builder •
          Banking & Finance Student
        </p>

      </div>

      <!-- FOOTER NAVIGATION -->
      <div class="footer-navigation">

        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#experience">Journey</a>
        <a href="#contact">Contact</a>

      </div>

      <!-- SOCIAL LINKS -->
      <div class="footer-social">

        <a
          href="https://github.com/"
          target="_blank"
          rel="noopener noreferrer"
          aria-label="GitHub"
        >
          GitHub
        </a>

        <a
          href="https://www.linkedin.com/"
          target="_blank"
          rel="noopener noreferrer"
          aria-label="LinkedIn"
        >
          LinkedIn
        </a>

        <a
          href="https://wa.me/2348093963715"
          target="_blank"
          rel="noopener noreferrer"
          aria-label="WhatsApp"
        >
          WhatsApp
        </a>

      </div>

    </div>


    <!-- DIVIDER -->
    <div class="footer-divider"></div>


    <!-- BOTTOM -->
    <div class="footer-bottom">

      <p>
        © {{ new Date().getFullYear() }}
        Adebayo Muh'sin Adebola.
        All rights reserved.
      </p>

      <a href="#home" class="back-top">
        Back to top ↑
      </a>

    </div>

  </footer>
</template>


<style scoped>

.footer {
  width: 100%;
  padding: 55px 7% 25px;

  background: #030611;

  border-top: 1px solid rgba(255, 255, 255, 0.06);
}


/* =================================
   MAIN FOOTER
================================= */

.footer-container {
  max-width: 1200px;
  margin: 0 auto;

  display: flex;
  align-items: center;
  justify-content: space-between;

  gap: 40px;
}


/* =================================
   BRAND
================================= */

.footer-brand {
  max-width: 300px;
}

.footer-logo {
  display: inline-block;

  color: #ffffff;

  text-decoration: none;

  font-size: 27px;
  font-weight: 900;
}

.footer-logo span {
  color: #3b82f6;
}

.footer-brand p {
  margin-top: 10px;

  color: #64748b;

  font-size: 12px;
  line-height: 1.6;
}


/* =================================
   NAVIGATION
================================= */

.footer-navigation {
  display: flex;

  align-items: center;

  justify-content: center;

  gap: 25px;

  flex-wrap: wrap;
}

.footer-navigation a {
  color: #94a3b8;

  text-decoration: none;

  font-size: 12px;

  font-weight: 700;

  transition: 0.3s ease;
}

.footer-navigation a:hover {
  color: #3b82f6;
}


/* =================================
   SOCIAL
================================= */

.footer-social {
  display: flex;

  align-items: center;

  gap: 18px;
}

.footer-social a {
  color: #94a3b8;

  text-decoration: none;

  font-size: 12px;

  font-weight: 700;

  transition: 0.3s ease;
}

.footer-social a:hover {
  color: #3b82f6;
}


/* =================================
   DIVIDER
================================= */

.footer-divider {
  max-width: 1200px;

  height: 1px;

  margin: 40px auto 20px;

  background: rgba(255, 255, 255, 0.06);
}


/* =================================
   BOTTOM
================================= */

.footer-bottom {
  max-width: 1200px;

  margin: 0 auto;

  display: flex;

  align-items: center;

  justify-content: space-between;

  gap: 20px;
}

.footer-bottom p {
  margin: 0;

  color: #475569;

  font-size: 11px;
}

.back-top {
  color: #64748b;

  text-decoration: none;

  font-size: 11px;

  font-weight: 800;

  transition: 0.3s ease;
}

.back-top:hover {
  color: #3b82f6;
}


/* =================================
   TABLET
================================= */

@media (max-width: 900px) {

  .footer-container {
    flex-wrap: wrap;

    justify-content: center;

    text-align: center;
  }

  .footer-brand {
    width: 100%;

    max-width: 500px;
  }

  .footer-navigation {
    width: 100%;
  }

  .footer-social {
    width: 100%;

    justify-content: center;
  }

}


/* =================================
   MOBILE
================================= */

@media (max-width: 550px) {

  .footer {
    padding: 50px 5% 22px;
  }

  .footer-container {
    flex-direction: column;

    gap: 25px;
  }

  .footer-navigation {
    gap: 15px 20px;
  }

  .footer-social {
    gap: 20px;
  }

  .footer-divider {
    margin-top: 30px;
  }

  .footer-bottom {
    flex-direction: column;

    justify-content: center;

    text-align: center;

    gap: 12px;
  }

}

</style>