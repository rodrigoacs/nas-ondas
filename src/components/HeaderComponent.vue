<template>
  <div class="background">
    <div class="container">
      <h1>logo</h1>
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
  padding: 0 80px;
  height: 140px;
}

.navs {
  display: flex;
  gap: 4rem;
}

.nav {
  color: #8d00d3;
  font-size: 24px;
  font-weight: 700;
  text-decoration: none;
}

.background {
  background-color: #f5c81e;
  opacity: 1;
  background-image: linear-gradient(#f4c014 0.7000000000000001px, transparent 0.7000000000000001px), linear-gradient(to right, #f4c014 0.7000000000000001px, #f5c81e 0.7000000000000001px);
  background-size: 14px 14px;
}
</style>