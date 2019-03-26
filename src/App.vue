<template>
  <div id="app">
    <h1>Conversor de moedas</h1>
    <div class="linha">
      <Conversor moedaA="USD" moedaB="BRL"></Conversor>
      <Conversor moedaA="BRL" moedaB="USD"></Conversor>
    </div>
    <div class="linha">
      <Conversor moedaA="USD" moedaB="EUR"></Conversor>
      <Conversor moedaA="EUR" moedaB="USD"></Conversor>
    </div>
    <div class="linha">
      <Conversor moedaA="EUR" moedaB="BRL"></Conversor>
      <Conversor moedaA="BRL" moedaB="EUR"></Conversor>
    </div>
  </div>
</template>

<script>
import Conversor from "./components/Conversor.vue";
export default {
  name: "app",
  components: {
    Conversor
  }
};
</script>

<style>
#app {
  max-width: 900px;
  margin: auto;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.linha {
  margin-top: 40px;
  display: flex;
  justify-content: space-between;
}
</style>
