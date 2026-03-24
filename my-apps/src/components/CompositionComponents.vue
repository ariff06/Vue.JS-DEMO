<script setup>
const firstName = "Arif"
const middleName = "Achmad"
const lastName = "Fauzy"

const showName = () => console.log(firstName + ' ' + middleName + ' ' + lastName)
</script>

<template>
    <h1>{{ firstName }}{{ middleName }}{{ lastName }}</h1>
    <button @click="showName">Show name!</button>
</template>