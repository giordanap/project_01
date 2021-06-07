<template>
    <h4>{{msg}}</h4>
 </template>

<script>
export default {
    name: 'Title',
    // Con esto podemos capturar el valor enviado.
    props: {
        msg: String
    }
}
</script>

<style scoped>
    h3 {
        color:steelblue;
    }
</style>