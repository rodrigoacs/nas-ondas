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
  width: 100%;
  max-width: 600px;
}

.card-image {
  width: 100%;
  height: 340px;
  border-radius: 12px;
  object-fit: cover;
}

.card-title {
  margin-top: 1rem;
  font-size: 1.3rem;
  font-weight: bold;
  color: var(--dark-purple);
  text-align: center;
}

@media (max-width: 768px) {
  .card {
    padding: 1rem;
  }

  .card-image {
    height: 260px;
  }

  .card-title {
    font-size: 1.1rem;
    margin-top: 0.8rem;
  }
}

@media (max-width: 480px) {
  .card {
    padding: 0.8rem;
  }

  .card-image {
    height: 200px;
  }

  .card-title {
    font-size: 1rem;
  }
}
</style>
