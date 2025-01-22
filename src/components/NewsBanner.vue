<template>
  <div class="background">
    <div class="container">
      <div class="horizontal-card">
        <img
          :src="image"
          alt="Imagem de destaque"
          class="card-image"
        />
        <div>
          <p class="card-header">{{ header }}</p>
          <p class="card-content">{{ content }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { defineProps } from 'vue'

const props = defineProps({
  image: String,
  header: String,
  content: String
})
</script>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 0 180px;
  height: 450px;
}

.background {
  background-color: var(--yellow);
  background-image: linear-gradient(#e39c0f 1px, transparent 1px),
    linear-gradient(to right, #e39c0f 1px, #e9ae18 1px);
  background-size: 20px 20px;
}

.horizontal-card {
  display: flex;
  align-items: center;
  gap: 1.5rem;
  border-radius: 12px;
  max-width: 80%;
}

.card-image {
  height: 310px;
  width: 100%;
  object-fit: cover;
  border-radius: 28px;
  border: 4px solid var(--purple);
}

.card-header {
  font-size: 1.6rem;
  line-height: 1.4;
  color: var(--purple);
  font-weight: bold;
}

.card-content {
  font-size: 1.2rem;
  line-height: 1.4;
  color: var(--black);
}
</style>