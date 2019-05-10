<template>
 
  <div id="app">
  <div class="titulo"><h1>Conversor de Moedas</h1></div>  
    <div class="linha">
    <Conversor moeda-a="USD" moeda-b="BRL"/>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
    <Conversor moeda-a="BRL" moeda-b="USD"/>  
  </div>
  </div>
</template>

<script>
import Conversor from "./components/Conversor.vue"

export default {
  name: 'app',
  components: {
    Conversor
  }
};
</script>

<style>
#app {
  margin: auto;
  max-width: 800px;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;   
  color: #2c3e50;
  margin-top: 60px;
}
.linha{
  background-color:darkseagreen;
  margin-top: 40px;
  display: flex;
  justify-content: space-around;
  border-radius: 90px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2); 
}
.titulo{
    text-align: center;
}
</style>
