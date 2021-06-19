<template>
    <h2>{{msg}}</h2>
 </template>

<script>
export default {
    name: 'Title',
    //You use 'prop' to capture the parameter sent by the component.
    props: {
        msg: String
    }
}
</script>

<style scoped>
    h2 {
        color:steelblue;
    }
</style>