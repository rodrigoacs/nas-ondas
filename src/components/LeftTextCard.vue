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
  padding: 1.5rem;
  background-color: var(--off-white);
  border-radius: 12px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
  max-width: 800px;
  margin: 0 auto;
}

.card-image {
  width: 120px;
  height: 120px;
  border-radius: 12px;
  object-fit: cover;
  border: 4px solid var(--purple);
}

.card-text {
  font-size: 1.6rem;
  line-height: 1.4;
  color: var(--dark-purple);
  font-weight: bold;
}
</style>
