<template>
  <div class="background">
    <div class="container">
      <div class="text-section">
        <p class="header">Como podemos te ajudar?</p>
        <p class="content">
          Não precisa se estressar com chatbots, filas de espera ou em ter que ficar abrindo vários tickets, é só ligar
          ou chamar no WhatsApp que a gente responde.
        </p>
      </div>
      <div class="contact-section">
        <div class="card">
          <div class="icon phone"></div>
          <div class="info">
            <p class="title">Telefone</p>
            <p class="detail">(31) 99999-9999</p>
          </div>
        </div>
        <div class="card">
          <div class="icon email"></div>
          <div class="info">
            <p class="title">E-mail</p>
            <p class="detail">nasondas@gmail.com</p>
          </div>
        </div>
        <div class="card whatsapp">
          <div class="icon whatsapp"></div>
          <div class="info">
            <p class="title">WhatsApp</p>
            <p class="detail">(31) 99999-9999</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
.background {
  background-color: var(--off-white);
  padding: 40px 0;
}

.container {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 0 20px;
  gap: 50px;
  text-align: center;
}

.text-section {
  width: 600px;
}

.text-section .header {
  font-size: 2.4rem;
  font-weight: bold;
  color: var(--purple);
  text-align: left;
}

.text-section .content {
  font-size: 1.1rem;
  color: #333;
  margin-top: 15px;
  text-align: justify;
}

.contact-section {
  display: grid;
  grid-template-columns: 1fr;
  gap: 20px;
  width: 100%;
  max-width: 400px;
}

.card {
  display: flex;
  align-items: center;
  background: var(--off-white);
  padding: 15px;
  border-radius: 10px;
  border: 3px solid var(--grey);
  gap: 15px;
}

.card.whatsapp {
  background: var(--green-wp);
  color: var(--white);
}

.icon {
  width: 50px;
  height: 50px;
  background-size: cover;
  background-position: center;
  border-radius: 5px;
}

.icon.phone {
  background-image: url('https://cdn-icons-png.flaticon.com/512/597/597177.png');
}

.icon.email {
  background-image: url('https://cdn-icons-png.flaticon.com/512/732/732200.png');
}

.icon.whatsapp {
  background-image: url('https://cdn-icons-png.flaticon.com/512/733/733585.png');
}

.info {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

.info .title {
  font-weight: bold;
  font-size: 1.2rem;
}

.info .detail {
  font-size: 1rem;
  margin-top: 5px;
}
</style>
