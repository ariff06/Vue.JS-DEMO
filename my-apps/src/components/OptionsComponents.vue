<script>
    export default {
        data() {
            return {
                firstName: 'Arif',
                middleName: 'Achmad',
                lastName: 'Fauzy'
        }
    },
        methods: {
            showName() {
                console.log(this.firstName + ' ' + this.middleName + ' ' + this.lastName)
        }
    }
}

</script>

<template>
    <h1>{{ firstName }}{{ middleName }}{{ lastName }}</h1>
    <button @click="showName">Show name!</button>    
</template>