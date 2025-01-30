<template>
  <div class="background">
    <div class="container">
      <div>
        <img
          src="../assets/quem-somos.avif"
          class="section-title"
          alt="Seção Quem Somos"
          loading="lazy"
        />
        <p class="content">
          Com mais de <b>30 anos de experiência</b> no mundo da comunicação, Luiz Evandro se destaca como <b>locutor,
            apresentador e mestre de cerimônias</b>, proporcionando uma presença única e marcante em eventos como
          <b>grandes shows, convenções, lançamentos de produtos, festa de 15 anos e formaturas.</b> Sua trajetória
          começou na <b>Rádio Congonhas</b> em 1993, trabalhou também nas <b>Rádio Inconfidência</b> de Belo Horizonte,
          <b>Rádio Educativa FM</b> em Congonhas e na <b>Rádio Colonial</b> FM onde desenvolveu uma habilidade
          impecável de <b> conectar-se com o público através da voz</b>, se tornando uma referência.

          Seu <b>estilo cativante</b>, aliado a uma excelente <b>capacidade de improviso e adaptação ao público</b>, o
          tornaram uma escolha de confiança para empresas e organizações que buscam qualidade e profissionalismo.

          Além de sua carreira como locutor e apresentador, Luiz Evandro também é conhecido por sua <b>habilidade em
            criar um ambiente acolhedor e envolvente, independentemente do porte do evento</b>. Sua energia contagiante
          e carisma são elementos que fazem de cada evento uma <b>experiência inesquecível</b>.
        </p>
      </div>
      <img
        src="/foto-bio.avif"
        class="profile-picture"
        alt="Foto de Luiz Evandro"
        loading="lazy"
      />
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
b {
  color: var(--highlight-color);
  font-weight: 700;
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 40px 180px;
  gap: 50px;
}

.background {
  background-color: var(--blue);
}

.section-title {
  width: 300px;
}

.content {
  color: var(--white);
  font-size: 20px;
  line-height: 30px;
  text-align: justify;
}

.profile-picture {
  height: 400px;
  object-fit: cover;
  border-radius: 26px;
}

@media (max-width: 768px) {
  .container {
    flex-direction: column;
    padding: 10px 20px;
    gap: 30px;
    height: auto;
  }

  .section-title {
    width: 100%;
    max-width: 250px;
    margin: 0 auto;
  }

  .content {
    width: 100%;
    max-width: 100%;
    font-size: 16px;
    line-height: 24px;
    text-align: justify;
  }

  .profile-picture {
    width: 100%;
    height: auto;
    margin: 0 auto;
  }
}

@media (max-width: 480px) {
  .content {
    font-size: 14px;
    line-height: 20px;
  }
}
</style>
