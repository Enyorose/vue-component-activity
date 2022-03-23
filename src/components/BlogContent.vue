<template>
  <section>
    <h1>{{ props.content.title }}</h1>
    <img :src="props.img.url" :alt="props.img.alt" />
    <p>{{ props.content.text }}</p>
  </section>
</template>

<script setup>
import { defineProps } from "vue";
const props = defineProps({
  content: {
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
section {
  display: flex;
  flex-direction: column;
}
</style>