<template>
  <div class="card-container">
    <img :src="props.img.url" :alt="props.img.alt" />
    <h1>{{ props.cardInfo.title }}</h1>
    <p>{{ props.cardInfo.cardText }}</p>
  </div>
</template>

<script setup>
import { defineProps } from "vue";
const props = defineProps({
  cardInfo: {
    type: Object,
  },
  img: {
    type: Object,
  },
});
</script>
<style scoped>
img {
  display: block;
  margin: 0 auto;
  max-width: 100%;
}
.card-container {
  display: flex;
  flex-direction: column;
  max-width: 30%;
  justify-content: center;
}
</style>