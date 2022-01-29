<template>
  <div id="menuBar">
      <nav>
          <div id="principal">
            <a href="#">Inicio</a>
            <a href="#">Nuestra historia</a>
            <a href="#">Catálogo</a>
            <a href="#">Pizzas</a>
          </div>
          <div id="login">
            <a href="#">Iniciar sesión</a>
            <a href="#">Registro</a>
          </div>
      </nav>
      
  </div>
</template>

<script>
export default {

}
</script>

<style>
#menuBar{
    background-color: lightblue;
}
nav{
    display: flex;
    justify-content: space-between;
    background-color: lightblue;
    padding: 1em 0em;
    font-weight: bold;
    margin: auto;
    max-width: 1400px;
}
    
    #principal a, #login a{
        padding: 1em 1.5em;
        text-decoration: none;
    }
    #menuBar a:hover{
        background-color: rgb(151, 216, 238);
        padding: 1.5em 2em;
        transition-duration: 0.2s;
        color: rgb(126, 8, 8);
    }
    #login a{
        background-color: rgb(105, 184, 105);
    }
    #login a:hover{
        background-color: rgb(134, 238, 134);
        color: blue;
        text-decoration: underline;
    }

    
</style>