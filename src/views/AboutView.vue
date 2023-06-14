<template>
  <div class="about">
    <h1>Conoce las Películas</h1>

    <div>
      <img alt="Vue logo" src="../assets/hp-1.jpeg">
      <img alt="Vue logo" src="../assets/hp-2.jpg" style="height: 267px; padding-left: 10px;">
      <img alt="Vue logo" src="../assets/hp-3.jpeg" style="height: 267px; padding-left: 10px;">
    </div>

    <p> {{ texto }} </p>
    <p> {{ peliculaBuscada }} </p>
    <input type="text" v-bind:value="contenidoTexto"><br>
    <button v-on:click="pelicula">Buscar</button>

  </div>
</template>

<script>

  export default{
    name: 'about-component',
    data: function(){
      return{
        texto: 'Resultado de búsqueda',
        peliculaBuscada: '',
        contenidoTexto: 'Busca una película'
      }
    },
    methods: {
      pelicula : function(){
        this.peliculaBuscada = 'Harry Potter y el Caliz del Fuego'
      }
    }
  }
</script>

<style scoped>

.about{
background-color: rgb(2, 7, 34);
color: #ffffff;
}

</style>