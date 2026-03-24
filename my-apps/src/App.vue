<script setup>
import MainButton from './components/MainButton.vue';
import CompositionComponents from './components/CompositionComponents.vue'
import OptionsComponents from './components/OptionsComponents.vue';
const firstName = "Arif";
const middleName = "Achamd";
const lastName = "Fauzy";
</script>

<template>
  <!-- With MainButton -->
  <MainButton></MainButton>
  <p>Mr. {{ firstName }} {{ middleName }} {{ lastName }}</p>

  <!-- With CompositionComponents -->
  <CompositionComponents></CompositionComponents>

  <!-- With OptionsComponenets -->
  <OptionsComponents></OptionsComponents>
</template>

<style scoped></style>