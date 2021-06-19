<template>
    <button 
        type="button" 
        :class=classButton
        @click="this.$emit('action')"
        :disabled="disabled"
    >
        {{ text }}
    </button>

</template>

<script>
export default {
    props: {
        text: String,
        // disabled: Boolean
        // Pero como el dato es dinamico, es recomendable tener un valor por defecto
        disabled: {
            type: Boolean,
            default: false
        }
    },
    computed: {
        classButton() {
            return this.text == "Increase Balance" ? "btn btn-secondary" : "btn btn-danger"
        }
    }
}
</script>

<style>

</style>