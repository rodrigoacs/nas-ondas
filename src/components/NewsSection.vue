<template>
  <div class="container">
    <img
      src="../assets/cafe.png"
      class="cafe"
    >
    <img
      src="../assets/noticias.png"
      class="section-title"
    >
    <img
      src="../assets/caneta.png"
      class="caneta"
    >
    <h1 class="subtitle">Notícias do Momento</h1>
    <div class="news1">
      <CardHightlight
        header="Amaury Lorenzo apresenta 'Hoje a festa é sua' direto de Congonhas na Rede Globo"
        content="Congonhas em destaque na chamada de fim de ano 'Hoje a festa é sua' na Rede Globo, com apresentação do Amaury Lorenzo"
        image="placeholder.png"
      />
      <div class="news2">
        <InnerTextCard
          header="Jubileu de Congonhas 2025"
          image="placeholder.png"
        />
        <InnerTextCard
          header="Limita uso de celulares nas escolas"
          image="placeholder.png"
        />
      </div>
    </div>
    <div class="news1">
      <BottomTextCard
        image="placeholder.png"
        title="Terremoto em Minas Gerais causa temor em Congonhas; barragem segue intacta"
      />
      <div class="news2">
        <LeftTextCard
          image="placeholder.png"
          text="Datafolha: 62% são contra anistia aos participantes do 8/1"
        />
        <LeftTextCard
          image="placeholder.png"
          text="Câmara conclui votação da primeira proposta do corte de gastos e derruba volta do DPVAT"
        />
      </div>
    </div>
    <NewsBanner
      image="placeholder.png"
      header="FNEC 2024 apontou o caminho do desenvolvimento sustentável de longo prazo para Congonhas - Correio de Minas"
      content="O Fórum Nacional de Educação e Cultura (FNEC) de 2024 apontou o caminho do desenvolvimento sustentável de longo prazo para Congonhas, com destaque para a educação e a cultura."
    />
  </div>
</template>

<script setup>
import CardHightlight from './CardHightlight.vue'
import InnerTextCard from './InnerTextCard.vue'
import BottomTextCard from './BottomTextCard.vue'
import LeftTextCard from './LeftTextCard.vue'
import NewsBanner from './NewsBanner.vue';

</script>

<style scoped>
.container {
  display: flex;
  position: relative;
  flex-direction: column;
  align-items: left;
  background-color: var(--off-white);
}

.news1 {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
  margin-top: 50px;
}

.news2 {
  display: flex;
  flex-direction: column;
  gap: 20px;
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
