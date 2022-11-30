<template>

    <div>
        {{$route.params.id}}
        Usuarios
    </div>

</template>

<script>
    export default {
        created() {
            console.log(this.$route);
        }
    }
</script>