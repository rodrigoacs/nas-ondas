<template>
  <footer class="footer">
    <div class="social-icons">
      <a
        href="https://www.instagram.com/nasondascomluizevandro/"
        target="_blank"
        class="icon instagram"
        aria-label="Visitar o perfil no Instagram"
      ></a>
      <a
        href="https://www.facebook.com/luizevandronasondasdoradio"
        target="_blank"
        class="icon facebook"
        aria-label="Visitar o perfil no Facebook"
      ></a>
      <a
        href="https://www.youtube.com/@luizevandronasondas2400"
        target="_blank"
        class="icon youtube"
        aria-label="Visitar o canal no YouTube"
      ></a>
    </div>
  </footer>
</template>

<script setup>
</script>

<style scoped>
.footer {
  background-color: var(--dark-purple);
  padding: 20px 0;
  display: flex;
  justify-content: center;
  align-items: center;
}

.social-icons {
  display: flex;
  gap: 20px;
}

.icon {
  width: 30px;
  height: 30px;
  background-size: cover;
  background-position: center;
  filter: brightness(0) invert(1);
  transition: transform 0.2s ease-in-out, opacity 0.2s ease-in-out;
}

.icon.instagram {
  background-image: url('https://cdn-icons-png.flaticon.com/512/174/174855.png');
}

.icon.facebook {
  background-image: url('https://cdn-icons-png.flaticon.com/512/2111/2111392.png');
}

.icon.youtube {
  background-image: url('https://cdn-icons-png.flaticon.com/512/3128/3128210.png');
}

.icon:hover {
  transform: scale(1.1);
  opacity: 0.8;
}

@media (max-width: 768px) {
  .icon {
    width: 25px;
    height: 25px;
  }

  .social-icons {
    gap: 15px;
  }
}

@media (max-width: 480px) {
  .icon {
    width: 20px;
    height: 20px;
  }

  .social-icons {
    gap: 10px;
  }
}
</style>
