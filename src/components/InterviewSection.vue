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
            class="video"
            src="https://www.youtube.com/embed/V9Cf_XlcYTg?autoplay=0"
            frameborder="0"
          />
          <iframe
            id="ytplayer"
            type="text/html"
            class="video"
            src="https://www.youtube.com/embed/V9Cf_XlcYTg?autoplay=0"
            frameborder="0"
          />
        </div>
        <div>
          <iframe
            id="ytplayer"
            type="text/html"
            class="video"
            src="https://www.youtube.com/embed/V9Cf_XlcYTg?autoplay=0"
            frameborder="0"
          />
          <iframe
            id="ytplayer"
            type="text/html"
            class="video"
            src="https://www.youtube.com/embed/V9Cf_XlcYTg?autoplay=0"
            frameborder="0"
          />
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
  flex-direction: column;
  align-items: left;
  padding-bottom: 10%;
}

.background {
  background-image: url('../assets/onda-cinza.png');
  background-size: cover;
  background-repeat: no-repeat;
}

.section-title {
  margin-top: 100px;
  margin-left: 280px;
  width: 300px;
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

iframe.video {
  width: 640px;
  height: 360px;
}

@media (max-width: 768px) {
  .section-title {
    margin-left: 0;
    margin-top: 50px;
    text-align: center;
  }

  .interviews {
    gap: 10px;
  }

  .interviews div {
    flex-wrap: wrap;
    gap: 10px;
  }

  iframe.video {
    max-width: 90%;
    height: auto;
    aspect-ratio: 16 / 9;
  }


}

@media (max-width: 480px) {
  .section-title {
    width: 250px;
  }

  iframe.video {
    max-width: 100%;
    height: auto;
    aspect-ratio: 16 / 9;
  }


}
</style>
