<template>

<div class="contenedor">
  <Cabecera />
</div>
  <MenuBar />
  <div class="contenedor">
  <Buscador />
  <Bread />
  <Articulo />
  <Descripcion />
</div>
  <Footer />
</template>

<script>

import Cabecera from "./components/Cabecera.vue"
import MenuBar from "./components/MenuBar.vue"
import Buscador from "./components/Buscador.vue"
import Bread from "./components/Bread.vue"
import Articulo from "./components/Articulo.vue"
import Descripcion from "./components/Descripcion.vue"
import Footer from "./components/Footer.vue"

export default {
  name: 'App',
  components: {
    Cabecera,
    MenuBar,
    Buscador,
    Bread,
    Articulo,
    Descripcion,
    Footer
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
  background-color: rgba(240, 240, 240, 0.363);
  
}
.contenedor{
  max-width: 1400px;
  margin: auto;
}
</style>
