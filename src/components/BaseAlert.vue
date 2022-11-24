<template>
    
    <div :class="baseClass">
    
        <slot/>

        <button @click="onClick">
            X
        </button>

    </div>

</template>


<script>
    export default {
        props: {
            variant: {
                type: String,
                default: ''
            }    
        },
        computed: {
            baseClass() {
                return [
                    'alert',
                    this.variant ? `alert-${this.variant}` : ''
                ]
            }
        },
        methods: {
            onClick() {
                // $emit envia dados para o PAI
                this.$emit('close');
                console.log("click");
            }
        }
    }
</script>


<style scoped>
    .alert {
        display: flex;
        justify-content: space-between;
        padding: 5px;
        border-radius: 6px;
        color: white;
        background: rgb(36, 39, 224);
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
    background: rgb(218, 8, 8);
    }

</style>