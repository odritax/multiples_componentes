<template>
  <div>
    <h3>{{titulo}}</h3>
    <ul>
      <li v-for="(enlace,i) in enlaces" v-bind:key="i">
        <a v-bind:href="enlace.url">{{enlace.texto}}</a>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: 'Listas',
  props:{
    titulo:String,
    enlaces:Array
  }
}
</script>
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
