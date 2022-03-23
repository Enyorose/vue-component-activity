<template>
  <main>
    <BlogContent :content="blogContent" :img="cardImage" />
    <ImageCard class="img-comp" :cardInfo="cardStuff" :img="cardImage" />
  </main>
</template>

<script setup>
import ImageCard from "./ImageCard.vue";
import BlogContent from "./BlogContent.vue";
const cardStuff = {
  title: "Home for the winter",
  cardText: "We made it back from arizona in a snow storm",
};
const cardImage = {
  url: "/cool-apartments.webp",
  alt: "This is a cool apartment building",
};
const blogContent = {
  title: "This is our super cool blog about our trip to arizona",
  text: "We had a great time in arizona we got tanned like lobster",
};
</script>
<style scoped>
main {
  display: flex;
  flex-direction: column;
  text-align: center;
  margin: 0 auto;
}
</style>