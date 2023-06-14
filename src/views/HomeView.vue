<template>
  <div class="home">
    <img v-bind:alt="textoMostrar" v-bind:src="imagenAMostrar">
    <button v-on:click="cargardobby">mostrar dobby</button>
    <button v-on:click="cargarharry">mostrar harry</button>
    <HelloWorld v-bind:msg= "mensaje" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  },
  data: function(){
    return{
      imagendobby: './assets/img/Dobby.webp',
      imagenHarry: './assets/img/harry.jpeg',
      imagenAMostrar: '',
      textoMostrar: 'No hay imagen seleccionada',
      mensaje: ''
    }
  },
  methods: {
    cargardobby: function(){
        this.imagenAMostrar = this.imagendobby;
        this.mensaje = "Dobby es un elfo libre"
    },
    cargarharry: function() {
      this.imagenAMostrar = this.imagenHarry;
      this.mensaje = "Expeliarmus"
    }
  }

}
</script>

<style>

.home{
background-color: rgb(6, 0, 14);
}

</style>
