<template>
    <header class="header">
        Header
    </header>
</template>

<script>
    export default {
         // antes de ser montado
        beforeMount() {
            // destruir as nossas libs
            // eventos
            // listeners
            console.log('beforeMount');
            console.log('Estado:', this.name);
            console.log('DOM:', this.$el);
        },

        // depois de montado
        mounted() {
            console.log('mounted');
            console.log('Estado:', this.name);
            console.log('DOM:', this.$el);
        }
    }
</script>

<style>
    .header{
        background-color: yellow;
        color: black;
    }
</style>