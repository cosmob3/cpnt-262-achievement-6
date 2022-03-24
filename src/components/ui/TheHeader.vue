<template>
  <header>
    <slot></slot>
    <h1>{{ pageInfo.title }}</h1>
    <img :src="props.img.url" alt="props.img.alt" />
    <p>{{ pageInfo.description }}</p>
  </header>
</template>

<script setup>
import { defineProps } from "vue";
const props = defineProps({
  pageInfo: {
    type: Object,
  },
  img: {
    type: Object,
    url: "",
    alt: "Extra Text",
  },
});
</script>

<style scoped>
header {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  background-color: rebeccapurple;
  color: ghostwhite;
}
img {
  max-width: 30rem;
}
</style>
