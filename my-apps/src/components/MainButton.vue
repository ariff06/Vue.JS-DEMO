<script setup>
    const fullName = "Arif Achmad Fauzy"
    const isLoading = true
    const buttonAttr = {
        disabled: isLoading,
    }

    const showName = () => console.log(fullName)
</script>

<template>
    <button v-bind="buttonAttr" :id="`id-${1}`" @click="showName">
        {{ isLoading ? 'Loading' : 'Submit'}}
    </button>
</template>

<style scoped></style>