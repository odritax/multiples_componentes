<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Listas titulo="Habilidades en Progreso" v-bind:enlaces="Habilidades_en_progreso"/>
    <Listas titulo="Mis Habilidaes" v-bind:enlaces="Habilidades"/>
  </div>
</template>
<script>
  import Listas from './components/Listas.vue'
  export default {
    name: 'App',
    components: {
      Listas
    },
    data: () => {
      return {
        Habilidades_en_progreso:[
          {texto:"CSS",url:"http://www.google.cl"},
          {texto:"Java Script 6",url:"http://www.youtube.com"},
          {texto:"VUE",url:"http://www.behance.com"},
          {texto:"Python",url:"http://www.twitter.com"}
        ],
        Habilidades:[
          {texto:"Cocinar",url:"http://www.tinder.com"},
          {texto:"Comer",url:"http://www.instagram.cl"},
          {texto:"Limpiar",url:"http://www.sesamo.com"}
        ]
      };
    }
  };
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
