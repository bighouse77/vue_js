<template>
    <header class="header">
        Header
    </header>
</template>

<script>
    export default {     
        // depois de montado
        mounted() {
            window.addEventListener('resize', this.resize);
        },
        
         // antes de ser montado
        beforeMount() {
            // destruir as nossas libs
            // eventos
            // listeners
            console.log('beforeMount');
            console.log('Estado:', this.name);
            console.log('DOM:', this.$el);
        },

        methods: {
            resize($evt) {
                console.log($evt);
            }
        }
        
    }
</script>

<style>
    .header{
        background-color: yellow;
        color: black;
    }
</style>