<template>
  <div class="card">
    <img
      :src="props.image"
      class="card-image"
    />
    <div class="card-overlay">
      <h2 class="card-header">{{ props.header }}</h2>
    </div>
  </div>
</template>

<script setup>
import { defineProps } from 'vue'

const props = defineProps({
  header: String,
  image: String
})
</script>

<style scoped>
.card {
  position: relative;
  width: 100%;
  width: 560px;
  height: 280px;
  overflow: hidden;
  border-radius: 12px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
}

.card-image {
  height: 300px;
  width: 100%;
  object-fit: cover;
}

.card-overlay {
  position: absolute;
  bottom: 0;
  width: 100%;
  padding: 1rem;
  background: linear-gradient(to top, rgba(0, 0, 0, 1), rgba(0, 0, 0, 0));
  color: white;
  text-align: center;
}

.card-header {
  font-size: 1.6rem;
  font-weight: bold;
  text-align: left;
  margin: 0;
}
</style>
