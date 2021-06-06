<template>
  <Navbar />
  <img alt="Vue logo" src="./assets/logo02.png">
  <HelloWorld msg="We are going to analyze your data."/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Navbar from './components/Navbar.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Navbar
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
