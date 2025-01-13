<template>
  <div class="container">
    <img
      src="../assets/cafe.png"
      class="cafe"
      alt="Café"
    >
    <img
      src="../assets/noticias.png"
      class="section-title"
      alt="Título Notícias"
    >
    <img
      src="../assets/caneta.png"
      class="caneta"
      alt="Caneta"
    >
    <h1 class="subtitle">Notícias do Momento</h1>
  </div>
</template>

<script setup>
</script>

<style scoped>
.container {
  display: flex;
  position: relative;
  flex-direction: column;
  align-items: left;
  background-color: var(--off-white);
}

.cafe {
  position: absolute;
  width: 350px;
  top: -20px;
  left: 0;
}

.section-title {
  margin-top: 100px;
  margin-left: 280px;
  width: 300px;
}

.caneta {
  position: absolute;
  width: 300px;
  top: 0px;
  right: 0px;
}

.subtitle {
  font-size: 1.8rem;
  font-weight: bold;
  color: var(--blue);
  text-align: right;
  margin-right: 280px;
}
</style>
