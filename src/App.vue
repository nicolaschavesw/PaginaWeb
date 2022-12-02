<template>
  <EncabezadoPagina/>
  <ContenidoPagina/>
  <RegistroProducto/>
</template>

<script>
import EncabezadoPagina from './components/EncabezadoPagina.vue';
import ContenidoPagina from './components/ContenidoPagina.vue';
import RegistroProducto from './components/RegistroProducto.vue';

export default {
  name: 'App',
  components: {
    EncabezadoPagina,
    ContenidoPagina,
    RegistroProducto,
  }
}
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
