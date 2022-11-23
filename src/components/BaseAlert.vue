<template>
    
    <div :class="`alert`">
        O seu formulário foi enviado com sucesso!
    </div>

</template>


<script>
    export default {
        props: ['variant']
    }
</script>



<style scoped>
    .alert {
        padding: 5px;
        border-radius: 6px;
        color: white;
        background: rgb(13, 129, 145);
    }
    .alert-success {
        padding: 5px;
        border-radius: 6px;
        color: white;
        background: rgb(8, 153, 52);
    }
    .alert-danger {
    padding: 5px;
    border-radius: 6px;
    color: white;
    background: rgb(8, 153, 52);
    }

</style>