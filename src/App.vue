<template>
  <div id="app">
    <the-header :pageInfo="pageInfo" :img="heroImage">
      <nav>
        <ul>
          <li>Home</li>
          <li>About</li>
          <li>Contact</li>
        </ul>
      </nav>
    </the-header>
    <main></main>
    <TheFooter />
  </div>
</template>

<script setup>
import TheHeader from "./components/base/TheHeader.vue";
import TheFooter from "./components/base/TheFooter.vue";

const pageInfo = {
  title: "Oops, I did it",
  description: "This is the landing page for our website",
};

const heroImage = {
  url: "https://images.pexels.com/photos/3831760/pexels-photo-3831760.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260",
  alt: "This is our beautiful image",
};
</script>

<style>
body {
  margin: 0;
}
main {
  display: flex;
  flex-direction: column;
  align-items: center;

  height: 80vh;
  margin: 0 auto;
  text-align: center;
}

nav ul {
  display: flex;
  justify-content: space-between;
  list-style-type: none;
  width: 80vw;
}
</style>
