<template>
  <ImageCard :cardInfo="cardInfo" :img="cardImage" />
</template>

<script setup>
import ImageCard from "./components/ImageCard.vue";

const cardInfo = {
  cardTitle: "Home for the winter",
  cardText: "We made it back from arizona in a snow storm",
};
const cardImage = {
  url: "https://images.unsplash.com/photo-1647533882992-c44e677b1cec?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1002&q=80",
  alt: "This is a cool apartment building",
};
</script>


