<template>
    <ul>
        <li v-for="stage in stages" :key="stage">{{stage}}</li>
    </ul>
</template>

<script>
export default {
    name: 'Processes',
    data() {
        return {
            stages: ['Admision','Comportamiento','Cobranzas']
        }
    }
}
</script>

<style>
    li {
        color: green;
    }
</style>