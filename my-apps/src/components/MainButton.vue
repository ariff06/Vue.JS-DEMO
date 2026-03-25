<script setup>
    const fullName = "Arif Achmad Fauzy"
    const buttonAttr = {
        disabled: true,
        id: 1,
    }

    const showName = () => console.log(fullName)
</script>

<template>
    <button v-bind="buttonAttr" @click="showName">This button will be disabled</button>
</template>

<style scoped></style>