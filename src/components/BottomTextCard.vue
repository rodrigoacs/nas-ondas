<template>
  <div class="card">
    <img
      :src="image"
      alt="Imagem de destaque"
      class="card-image"
    />
    <p class="card-title">{{ title }}</p>
  </div>
</template>

<script setup>
import { defineProps } from 'vue'

const props = defineProps({
  image: String,
  title: String,
})
</script>

<style scoped>
.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: var(--light-gray, #f5f5f5);
  padding: 1.5rem;
  border-radius: 12px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  width: 100%;
  max-width: 600px;
  margin: 0 auto;
}

.card-image {
  width: 100%;
  height: auto;
  border-radius: 12px;
  /* Bordas arredondadas */
  object-fit: cover;
}

.card-title {
  margin-top: 1rem;
  font-size: 1.6rem;
  font-weight: bold;
  color: var(--dark-purple);
  /* Cor do texto */
  text-align: center;
}
</style>
