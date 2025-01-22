<template>
  <div class="background">
    <div class="container">
      <img
        src="../assets/entrevistas.png"
        class="section-title"
      >
      <div class="interviews">
        <div>
          <iframe
            id="ytplayer"
            type="text/html"
            width="640"
            height="360"
            src="http://www.youtube.com/embed/V9Cf_XlcYTg?autoplay=0&origin=http://example.com"
            frameborder="0"
          />
          <iframe
            id="ytplayer"
            type="text/html"
            width="640"
            height="360"
            src="http://www.youtube.com/embed/V9Cf_XlcYTg?autoplay=0&origin=http://example.com"
            frameborder="0"
          /><iframe
            id="ytplayer"
            type="text/html"
            width="640"
            height="360"
            src="http://www.youtube.com/embed/V9Cf_XlcYTg?autoplay=0&origin=http://example.com"
            frameborder="0"
          />
        </div>
        <div>
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
}

.background {
  background-image: url('../assets/onda-cinza.png');
}

.section-title {
  margin-top: 100px;
  margin-left: 280px;
  width: 300px;
}

img {
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
