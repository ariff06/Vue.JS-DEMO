<script setup>
    const fullName = "Arif Achmad Fauzy"
    const isLoading = false
    const buttonAttr = {
        disabled: isLoading,
        id: 1
    }
    const renderIsLoading = () => {
        if (isLoading) {
            return 'Loading'
        } else {
            return 'Sumbit'
        }
    }

    const showName = () => console.log(fullName)
</script>

<template>
    <button v-bind="buttonAttr" :id="`id-${buttonAttr.id}`" @click="showName">
        {{ renderIsLoading() }}
    </button>
</template>

<style scoped></style>