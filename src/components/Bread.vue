<template>
  <div id="bread">
      <a href="#">Inicio</a>
      <span>></span>
      <a href="#">Catálogo</a>
      <span>></span>
      <a href="#" id="actual">Pizzas 4 ingredientes</a>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    #bread{
        text-align: left;
        margin-bottom: 1em;
    }
    #bread a{
        padding: 1em 1.5em;
        text-decoration: none;
    }

    #bread a:hover{
        text-decoration: underline;
        color: rgb(255, 67, 67);
    }
    #actual{
        font-weight: bold;
    }
</style>