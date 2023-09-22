<template>
  <div class="hello">
    {{ count }}
    <button @click="increment">Adicionar</button><button @click="reset">Resetar</button>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  name: 'CountAdder',
  props: {
    msg: String
  },
  setup(){
    const count = ref(0);

    function increment(){
      count.value++;
    }

    function reset(){
      count.value = 0;
    }

    return {
      count, increment, reset
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
