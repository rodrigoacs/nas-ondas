<template>
  <div class="container">
    <h1 class="header">
      {{ props.header }}
    </h1>
    <p class="content">
      {{ props.content }}
    </p>
    <img
      :src="props.image"
      alt="Imagem de destaque"
    />
  </div>
</template>

<script setup>
import { defineProps } from 'vue'

const props = defineProps({
  header: String,
  content: String,
  image: String
})
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1.5rem;
  padding: 2rem;
  max-width: 100%;
  width: 600px;
  background-color: var(--highlight-color) !important;
  border-radius: 12px;
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
}

.header {
  font-size: 1.6rem;
  font-weight: bold;
  color: var(--dark-purple);
  text-align: justify;
  line-height: 1.2;
}

.content {
  font-size: 1.2rem;
  line-height: 1.4;
  color: var(--black);
  text-align: justify;
}

img {
  max-width: 100%;
  height: 300px;
  width: 100%;
  object-fit: cover;
  border-radius: 8px;
  border-color: var(--purple);
  border-width: 4px;
  border-style: solid;
}
</style>
