<template>
  <div class="background">
    <div class="container">
      <img
        class="decor-azul"
        src="../assets/decor-azul.svg"
      >
      <img
        class="decor-amarelo"
        src="../assets/decor-amarelo.svg"
      >
      <img
        src="../assets/eventos.avif"
        class="section-title"
      >
      <div class="interviews">
        <div>
          <img
            src="https://i.ytimg.com/vi/j_nhsENynDs/hq720.jpg?sqp=-oaymwEnCNAFEJQDSFryq4qpAxkIARUAAIhCGAHYAQHiAQoIGBACGAY4AUAB&rs=AOn4CLAlPEL8_okigWOGvgx80kcd1GlhbQ"
          >
          <img
            src="https://i.ytimg.com/vi/j_nhsENynDs/hq720.jpg?sqp=-oaymwEnCNAFEJQDSFryq4qpAxkIARUAAIhCGAHYAQHiAQoIGBACGAY4AUAB&rs=AOn4CLAlPEL8_okigWOGvgx80kcd1GlhbQ"
          >
          <img
            src="https://i.ytimg.com/vi/j_nhsENynDs/hq720.jpg?sqp=-oaymwEnCNAFEJQDSFryq4qpAxkIARUAAIhCGAHYAQHiAQoIGBACGAY4AUAB&rs=AOn4CLAlPEL8_okigWOGvgx80kcd1GlhbQ"
          >
        </div>
        <div>
          <img
            src="https://i.ytimg.com/vi/j_nhsENynDs/hq720.jpg?sqp=-oaymwEnCNAFEJQDSFryq4qpAxkIARUAAIhCGAHYAQHiAQoIGBACGAY4AUAB&rs=AOn4CLAlPEL8_okigWOGvgx80kcd1GlhbQ"
          >
          <img
            src="https://i.ytimg.com/vi/j_nhsENynDs/hq720.jpg?sqp=-oaymwEnCNAFEJQDSFryq4qpAxkIARUAAIhCGAHYAQHiAQoIGBACGAY4AUAB&rs=AOn4CLAlPEL8_okigWOGvgx80kcd1GlhbQ"
          >
          <img
            src="https://i.ytimg.com/vi/j_nhsENynDs/hq720.jpg?sqp=-oaymwEnCNAFEJQDSFryq4qpAxkIARUAAIhCGAHYAQHiAQoIGBACGAY4AUAB&rs=AOn4CLAlPEL8_okigWOGvgx80kcd1GlhbQ"
          >
        </div>
      </div>
    </div>
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
  padding-bottom: 10%;
  overflow: hidden;
}

.section-title {
  margin-top: 100px;
  margin-left: 280px;
  width: 300px;
}

.decor-azul {
  position: absolute;
  top: 650px;
  left: -200px;
  z-index: 1;
}

.decor-amarelo {
  position: absolute;
  bottom: -250px;
  right: -150px;
  z-index: -1;
  filter: hue-rotate(-40deg)
}

.interviews img {
  width: 500px;
  height: 100%;
}

.interviews {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 20px;
  margin-top: 50px;
}

.interviews div {
  display: flex;
  gap: 20px;
}
</style>
