<script setup>
import MainButton from './components/MainButton.vue';
const firstName = "Arif";
const middleName = "Achamd";
const lastName = "Fauzy";
</script>

<template>
  <!-- With MainButton -->
  <MainButton></MainButton>
  <p>Mr. {{ firstName }} {{ middleName }} {{ lastName }}</p>

  <!-- Added at main.js -->
  <CompositionComponents />
  <!-- Added at main.js -->
  <OptionsComponents />
</template>

<style scoped></style>
