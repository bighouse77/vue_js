<template>
    <header class="header">
        
        <h1 v-if="$slots.title" class="title">
            <slot name="title"/>
        </h1>
        
        <div class="description">
            <slot name="description"/>
        </div>
        
        <div class="content">
            <slot/>
        </div>

    </header>
</template>

<script>
    export default {     
        // depois de montado
        mounted() {
            console.log(this.$slots);
        },
    }
</script>

<style>
    .header{
        background-color: black;
        color: white;
    }
</style>