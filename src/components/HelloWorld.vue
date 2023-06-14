<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Para una guia sobre como configurar este proyecto:<br>
      revisa el siguiente enlace:
      <a href="https://cli.vuejs.org" target="_blank" rel="noopener">vue-cli documentation</a>.
    </p>
    <h3>Personajes Principales</h3>
    <ul>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-router" target="_blank" rel="noopener">Harry Potter</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-vuex" target="_blank" rel="noopener">Hermiones Granger</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-vuex" target="_blank" rel="noopener">Ron Weasley</a></li>
    </ul>

    <h3>Personajes antagonistas</h3>
    <ul>
      <li><a href="https://router.vuejs.org" target="_blank" rel="noopener">Voldemort</a></li>
      <li><a href="https://vuex.vuejs.org" target="_blank" rel="noopener">Bellatrix Lestrange</a></li>
      <li><a href="https://github.com/vuejs/vue-devtools#vue-devtools" target="_blank" rel="noopener">Draco Malfoy</a></li>
      <li><a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener">Profesor Quirrell</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello{
  background-color: rgb(1, 4, 23);
}

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
  color: #8a76f7;
}
</style>
