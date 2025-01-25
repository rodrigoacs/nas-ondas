<template>
  <div class="background">
    <div class="container">
      <div class="text-section">
        <p class="header">Entre em contato!</p>
      </div>
      <div class="contact-section">
        <a
          href="https://wa.me/5531982676163"
          target="_blank"
          class="card whatsapp"
        >
          <div class="icon whatsapp"></div>
          <div class="info">
            <p class="title">WhatsApp</p>
            <p class="detail">(31) 98267-6163</p>
          </div>
        </a>

        <a
          href="tel:+5531982676163"
          class="card"
        >
          <div class="icon phone"></div>
          <div class="info">
            <p class="title">Telefone</p>
            <p class="detail">(31) 98267-6163</p>
          </div>
        </a>

        <a
          href="mailto:nasondasdoradio1020@gmail.com"
          class="card"
        >
          <div class="icon email"></div>
          <div class="info">
            <p class="title">E-mail</p>
            <p class="detail">nasondasdoradio1020@gmail.com</p>
          </div>
        </a>
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
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 0 20px;
  gap: 30px;
  text-align: center;
}

.text-section {
  width: 600px;
}

.text-section .header {
  font-size: 2.4rem;
  font-weight: bold;
  color: var(--purple);
  text-align: center;
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
  text-decoration: none;
  /* Remove underline dos links */
  color: inherit;
  /* Herda a cor para manter o estilo */
  transition: transform 0.2s ease;
}

.card:hover {
  transform: scale(1.05);
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

/* Responsividade */
@media (max-width: 768px) {
  .text-section {
    width: 90%;
  }

  .text-section .header {
    font-size: 2rem;
  }

  .contact-section {
    max-width: 100%;
    grid-template-columns: 1fr;
    gap: 15px;
  }

  .card {
    padding: 10px;
  }

  .icon {
    width: 40px;
    height: 40px;
  }

  .info .title {
    font-size: 1rem;
  }

  .info .detail {
    font-size: 0.9rem;
  }
}

@media (max-width: 480px) {
  .text-section .header {
    font-size: 1.8rem;
  }

  .icon {
    width: 35px;
    height: 35px;
  }

  .info .title {
    font-size: 0.9rem;
  }

  .info .detail {
    font-size: 0.8rem;
  }
}
</style>
