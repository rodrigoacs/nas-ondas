<template>
  <div class="background">
    <div class="container">
      <a
        href="#home"
        class="logo-link"
      >
        <img
          class="logo"
          src="../assets/logo-texto.avif"
          alt="Logo"
        />
      </a>
      <div class="navs">
        <a
          href="#interview"
          class="nav-item"
        >
          <span class="nav-text">ENTREVISTAS</span>
          <img
            src="https://cdn-icons-png.flaticon.com/512/1436/1436769.png"
            alt="Entrevistas"
            class="icon"
          />
        </a>
        <a
          href="#about"
          class="nav-item"
        >
          <span class="nav-text">QUEM SOMOS?</span>
          <img
            src="https://cdn-icons-png.flaticon.com/512/681/681494.png"
            alt="Quem Somos"
            class="icon"
          />
        </a>
        <a
          href="#contact"
          class="nav-item"
        >
          <span class="nav-text">CONTATO</span>
          <img
            src="https://cdn-icons-png.flaticon.com/512/8485/8485251.png"
            alt="Contato"
            class="icon"
          />
        </a>
      </div>
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 10%;
  height: 80px;
}

.logo-link {
  text-decoration: none;
  display: flex;
}

.logo {
  max-width: 100%;
  height: 70px;
  object-fit: contain;
  justify-self: flex-start;
}

.navs {
  display: flex;
  align-items: center;
  gap: 2rem;
}

.nav-item {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  text-decoration: none;
  color: var(--purple);
  font-size: 1.2rem;
}

.nav-text {
  display: inline;
  font-weight: 700;
}

.icon {
  display: none;
  width: 20px;
  height: 20px;
  object-fit: contain;
  filter: brightness(0) saturate(100%) invert(18%) sepia(94%) saturate(1732%) hue-rotate(250deg) brightness(92%) contrast(85%);
}

.background {
  background-color: var(--yellow);
  background-image: linear-gradient(#e39c0f 1px, transparent 1px),
    linear-gradient(to right, #e39c0f 1px, #e9ae18 1px);
  background-size: 20px 20px;
}

@media (max-width: 768px) {
  .nav-text {
    display: none;
  }

  .icon {
    display: block;
    width: 20px;
    height: 20px;
  }
}

@media (max-width: 480px) {
  .icon {
    width: 20px;
    height: 20px;
  }
}
</style>
