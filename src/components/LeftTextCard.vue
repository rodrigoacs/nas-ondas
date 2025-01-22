<template>
  <div class="horizontal-card">
    <img
      :src="image"
      alt="Imagem de destaque"
      class="card-image"
    />
    <p class="card-text">{{ text }}</p>
  </div>
</template>

<script setup>
import { defineProps } from 'vue'

const props = defineProps({
  image: String,
  text: String,
})
</script>

<style scoped>
.horizontal-card {
  display: flex;
  align-items: center;
  gap: 1.5rem;
  background-color: var(--off-white);
  border-radius: 12px;
  max-width: 600px;
}

.card-image {
  width: 180px;
  height: 140px;
  border-radius: 12px;
  object-fit: cover;
  border: 4px solid var(--purple);
}

.card-text {
  font-size: 1.3rem;
  line-height: 1.4;
  color: var(--dark-purple);
  font-weight: bold;
}
</style>
