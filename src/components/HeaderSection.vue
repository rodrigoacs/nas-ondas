<template>
  <div class="background">
    <div class="container">
      <img
        class="logo"
        src="../assets/logo-texto.png"
      >
      <div class="navs">
        <a href="#home"> INÍCIO </a>
        <!-- <a href="#news"> NOTICIAS </a> -->
        <a href="#interview"> ENTREVISTAS </a>
        <a href="#about">QUEM SOMOS?</a>
        <a href="#contact">CONTATO</a>
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
  padding: 0 180px;
  height: 80px;
}

.logo {
  max-width: 100%;
  height: 70px;
  object-fit: contain;
}

.navs {
  display: flex;
  align-items: center;
  gap: 3rem;
}

.navs a {
  color: var(--purple);
  font-size: 24px;
  font-weight: 700;
  text-decoration: none;
}

.background {
  background-color: var(--yellow);
  background-image: linear-gradient(#e39c0f 1px, transparent 1px),
    linear-gradient(to right, #e39c0f 1px, #e9ae18 1px);
  background-size: 20px 20px;
}

/* Responsividade */
@media (max-width: 768px) {
  .container {
    padding: 0 20px;
    height: auto;
    flex-direction: column;
    gap: 1rem;
    text-align: center;
  }

  .logo {
    height: 60px;
  }

  .navs {
    display: none;
  }

  .navs a {
    font-size: 20px;
  }
}

@media (max-width: 480px) {
  .container {
    padding: 5px 10px;
    gap: 1rem;
  }

  .logo {
    height: 50px;
  }

  .navs a {
    font-size: 18px;
  }
}
</style>
