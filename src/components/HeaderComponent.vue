<template>
  <div class="background">
    <div class="container">
      <img
        class="logo"
        src="../assets/logo-texto.png"
      >
      <div class="navs">
        <a class="nav">INÍCIO</a>
        <a class="nav">REPORTAGENS</a>
        <a class="nav">ENTREVISTAS</a>
        <a class="nav">CONTATO</a>
        <a class="nav">SOBRE NÓS</a>
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
  height: 140px;
}

.logo {
  width: 260px;
  object-fit: contain;
}

.navs {
  display: flex;
  align-items: center;
  gap: 3rem;
}

.nav {
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
</style>