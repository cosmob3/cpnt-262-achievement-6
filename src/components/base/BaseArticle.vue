<template>
  <h2>Co-Workers and Their Specialties</h2>
  <ul>
    <li v-for="partners in store" :key="partners.id">
      {{ partners.name }} -- {{ partners.specialty }}
    </li>
  </ul>
</template>

<script setup>
const store = [
  {
    name: "Izzy",
    specialty: "Everything",
  },
  {
    name: "Maddox",
    specialty: "Drive-Thru",
  },
  {
    name: "Joel",
    specialty: "Customer Connections",
  },
  {
    name: "Lyddia",
    specialty: "Bar",
  },
  {
    name: "Trinity",
    specialty: "Customer Service",
  },
  {
    name: "Chloe",
    specialty: "Knows a little bit about everything",
  },
];
</script>

<style scoped>
h2 {
  font-size: 50px;
}
ul {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  background-color: green;
  color: ghostwhite;
  font-size: 30px;
  padding: 5rem;
}
</style>
