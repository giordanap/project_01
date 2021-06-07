<template>
  <Title msg="We are going to analyze your data."/>
  <img alt="Vue logo" src="./assets/logo02.png">
  <hr>
  <Processes/>

</template>

<script>
import Title from './components/Title.vue'
import Processes from './components/Processes.vue'

export default {
  name: 'App',
  components: {
    Title, Processes
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
