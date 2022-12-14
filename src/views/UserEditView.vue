<template>

    <div>
        {{$route.params.id}}
        Usuarios

        <br>

        <button @click="login()">
            Login
        </button>

    </div>
 
</template>

<script>
    export default {
        created() {
            console.log(this.$router);
        },

        methods: {
            login(){
                // ajax login
                this.$router.push({ name: 'about' });
                console.log("clicou");
            }
        }
    }
</script>