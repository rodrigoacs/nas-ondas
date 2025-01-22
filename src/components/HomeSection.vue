<template>
  <section>
    <div class="banner-container">
      <img src="../assets/banner-home.jpg" />
      <div class="banner-content">
        <p class="main-text">
          <strong>Bem-vindo</strong> ao espaço onde cada palavra amplifica sua mensagem.
          Conecte-se <strong>Nas Ondas com Luiz Evandro</strong> e potencialize eventos e campanhas.
        </p>
        <p class="sub-text">Explore nossos serviços de locução para eventos, companhas publicitárias, cerimônias e muito
          mais.</p>
        <button class="more-info"><a href="#about">Saiba mais</a></button>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
a {
  text-decoration: none;
  font-size: 1.6rem;
  font-weight: 700;
}

.banner-container {
  position: relative;
  width: 100%;
  height: auto;
}

img {
  width: 100%;
  display: block;
}

.banner-content {
  position: absolute;
  top: 40%;
  width: 50rem;
  color: #fff;
  padding-left: 10rem;
}

.main-text {
  font-size: 2.8rem;
  line-height: 1.2;
  text-shadow: 0 2px 4px rgba(0, 0, 0, 0.5);
}

.main-text strong {
  font-weight: 700;
}

.more-info {
  background: linear-gradient(90deg, #e7a617 0%, #ffd500 100%);
  color: var(--purple);

  padding: 1.5rem 3rem;
  margin-top: 4rem;
  border: none;
  border-radius: 1000px;
  cursor: pointer;
}

.sub-text {
  font-size: 1.4rem;
  line-height: 1.2;
  margin-top: 2rem;
  text-shadow: 0 2px 4px rgba(0, 0, 0, 0.5);
}
</style>
