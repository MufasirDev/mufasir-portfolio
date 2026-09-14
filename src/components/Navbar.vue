<template>
  <nav class="navbar">
    <div class="nav-container">
      <a href="#home" class="logo">
        <span>M</span>ufasir <span>D</span>ev
      </a>

      <div class="nav-links">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#experience">Experience</a>
        <a href="#contact">Contact</a>
      </div>

      <a href="#contact" class="nav-button">
        Let's Talk
      </a>
    </div>
  </nav>
</template>

<style scoped>
.navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1000;
  padding: 22px 7%;
  background: rgba(5, 10, 25, 0.9);
  backdrop-filter: blur(14px);
  border-bottom: 1px solid rgba(255, 255, 255, 0.06);
}

.nav-container {
  max-width: 1300px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo {
  color: #ffffff;
  font-size: 28px;
  font-weight: 800;
  text-decoration: none;
}

.logo span {
  color: #3b82f6;
}

.nav-links {
  display: flex;
  align-items: center;
  gap: 32px;
}

.nav-links a {
  color: #cbd5e1;
  text-decoration: none;
  font-size: 15px;
  font-weight: 600;
  transition: 0.3s ease;
}

.nav-links a:hover {
  color: #3b82f6;
}

.nav-button {
  color: #ffffff;
  background: #2563eb;
  padding: 12px 22px;
  border-radius: 8px;
  text-decoration: none;
  font-weight: 700;
  transition: 0.3s ease;
}

.nav-button:hover {
  background: #1d4ed8;
  transform: translateY(-2px);
}

@media (max-width: 850px) {
  .nav-links {
    display: none;
  }

  .nav-button {
    padding: 10px 17px;
    font-size: 14px;
  }
}
</style>