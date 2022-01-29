<template>
  <div id="buscador">
      <form action="#">
          <input type="text" class="buscador" id="inputBuscar" placeholder="Buscar productos ..." />
          <input type="submit" class="buscador" id="botonBuscar" value="Buscar" />
      </form>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    #buscador{
        display: flex;
        justify-content: center;
        margin: 2em 0em;
    }

    .buscador{
        font-size: 1.3em;
        margin-right: 1em;
    }

    #inputBuscar{
        border-radius: 1em;
        border-color: rgb(62, 233, 255);
        padding: 0.3em;
    }

    #botonBuscar, #carrito{
        padding: 0.4em 1em;
        background-color: lightblue;
        border-color: transparent;
    }

   

</style>