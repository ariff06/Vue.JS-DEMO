<script setup>
    const fullName = "Arif Achmad Fauzy"
    const isLoading = true
    const buttonAttr = {
        disabled: isLoading,
        id: 1
    }

    const showName = () => console.log(fullName)
</script>

<template>
    <button v-bind="buttonAttr" :id="`id-${buttonAttr.id}`" @click="showName">
        {{ isLoading ? 'Loading' : 'Submit'}}
    </button>
</template>

<style scoped></style>