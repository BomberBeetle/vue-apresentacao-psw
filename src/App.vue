<template>
  <h3>Olá Vue!</h3>

  <Adder msg="Welcome to Your Vue.js App"/>
  <Adder msg="Welcome to Your Vue.js App"/>
  <Adder msg="Welcome to Your Vue.js App"/>
  <Adder msg="Welcome to Your Vue.js App"/>
</template>

<script>
import Adder from './components/Adder.vue'

export default {
  name: 'BigApp',
  components: {
    Adder
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
