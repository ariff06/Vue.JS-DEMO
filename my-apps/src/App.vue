<script setup>
import MainButton from './components/MainButton.vue'
const firstName = "Arif"
const middleName = "Achamd"
const lastName = "Fauzy"
const blogSpot = '<h1 style="color:blue">I like blue color!</h1>'
const idBlog = 'blog-01'
</script>

<template>
  <!-- With MainButton -->
  <MainButton></MainButton>
  <p>Mr. {{ firstName }} {{ middleName }} {{ lastName }}</p>
  <!-- Added at main.js -->
  <CompositionComponents />
  <!-- Added at main.js -->
  <OptionsComponents />

  <!-- Text interpolation -->
  <div :id="idBlog">
    {{ blogSpot }}
  </div>
  <!-- rawHTML -->
   <div v-html="blogSpot"></div>
</template>

<style scoped></style>
