<template>
  <div id="app">
    <nav>
      <router-link to="/">Personajes</router-link> |
      <router-link to="/about">Películas</router-link>
    </nav>
    <router-view/>

    <hr>
    <div class="prueba">
    <h3>Contenido:</h3>
    <p class="parrafoMensaje"> {{ mensaje }}</p>
  </div>
  </div>
</template>

<script>
  export default{
    name: 'app-component',
    data: function(){
      return{
        mensaje:'hola con vue',
        saludo: ''
      }
    },
    methods: {
      saludar: function(){
        this.saludo = 'Estoy cambiando una propiedad del modelo de datos';
      }
    }
  }
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #f1f1f1;
}

body{
 background-color: rgb(8, 2, 43);
 }

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #fafafa;
}

nav a.router-link-exact-active {
  color: #efe11f;
}

.parrafoMensaje{
  font-size: 20px;
}

</style>
