<script setup>
const props = defineProps(['title'])

    const showName = () => console.log(fullName)
</script>

<template>
    <button @click="showName">
        {{ props.title }}
    </button>
</template>

<style scoped></style>