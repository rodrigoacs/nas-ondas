<template>
  <div class="banner-container">
    <img
      id="banner"
      :src="imageSrc"
    />
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
</template>

<script setup>
import { ref, onMounted, onUnmounted, computed } from 'vue'

const windowWidth = ref(window.innerWidth)

const handleResize = () => {
  windowWidth.value = window.innerWidth
}

onMounted(() => {
  window.addEventListener('resize', handleResize)
})

onUnmounted(() => {
  window.removeEventListener('resize', handleResize)
})

const imageSrc = computed(() => windowWidth.value <= 768 ? '/banner-home-mobile.avif' : '/banner-home.avif')
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
  height: 100vh;
  overflow: hidden;
}

img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.banner-content {
  position: absolute;
  top: 40%;
  left: 10%;
  width: 50rem;
  color: #fff;
  padding: 0 2rem;
}

.main-text {
  font-size: 2.2rem;
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
  text-align: justify;
}

@media (max-width: 768px) {
  img {
    object-position: left;
  }

  .banner-content {
    top: 50%;
    left: 5%;
    width: 90%;
    padding: 0;
    transform: translateY(-50%);
  }

  .main-text {
    font-size: 2rem;
    line-height: 1.4;
  }

  .sub-text {
    font-size: 1.2rem;
    margin-top: 1.5rem;
  }

  .more-info {
    padding: 1rem 2rem;
    font-size: 1.2rem;
  }
}

@media (max-width: 480px) {
  .banner-content {
    top: 55%;
    width: 95%;
    padding: 0 1rem;
    transform: translateY(-50%);
  }

  .main-text {
    font-size: 1.6rem;
  }

  .sub-text {
    font-size: 1rem;
  }

  .more-info {
    padding: 0.8rem 1.5rem;
    font-size: 1rem;
  }
}
</style>
