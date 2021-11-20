<template>
  <div id="app">
    <div class="text-center">
      <h1>Conversor de Moedas</h1>
    </div>
    <div class="linha">
      <Conversor moedaA="USD" moedaB="BRL"/>
      <Conversor moedaA="BRL" moedaB="USD"/>
    </div>
    <div class="linha">
      <Conversor moedaA="EUR" moedaB="BRL"/>
      <Conversor moedaA="BRL" moedaB="EUR"/>
    </div>
    <div class="linha">
      <Conversor moedaA="CAD" moedaB="BRL"/>
      <Conversor moedaA="BRL" moedaB="CAD"/>
    </div>
  </div>
</template>

<script>
import Conversor from "./components/Conversor.vue";
export default{
  name: "app",
  components: {
    Conversor
  }
};
</script>

<style>
#app{
  margin: auto;
  max-width: 900px;
  text-align: center;
  margin-top: 60px;
}
.linha{
  display: flex;
  justify-content: space-around;
  margin-top: 40px;
}
</style>