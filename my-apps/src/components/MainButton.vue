<script setup>
    const fullName = "Arif Achmad Fauzy"
    const isLoading = false
    const buttonAttr = {
        type: 'button',
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
    const url = {
        attr: 'href',
        linkOne: '/home',
        linkTwo: '/dashboard'
    }

    const showName = () => console.log(fullName)
</script>

<template>
    <a :[url.attr]="url.linkTwo">
        <button v-bind="buttonAttr" :id="`id-${buttonAttr.id}`" @click="showName">
            {{ renderIsLoading() }}
        </button>
    </a>
</template>

<style scoped></style>