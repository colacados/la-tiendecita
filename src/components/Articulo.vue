<template>
<Icon path="{mdiCartArrowDown}" />
<Icon path="{mdiCartArrowDown}" />
<Icon path="{mdiCartArrowDown}" />
<mdiCartArrowDown />
  <div id="main">
      <div id="imagenes">
        <img width="400" id="imgprincipal" src="../assets/pizza1.png" >
        <div id="miniaturas">
            <img class="imgpeq" @click="ampliarImg('img1')" id="img1" src="../assets/pizza1.png" >
            <img class="imgpeq" @click="ampliarImg('img2')" id="img2" src="../assets/pizza2.jpg" >
            <img class="imgpeq" @click="ampliarImg('img3')" id="img3" src="../assets/pizza3.jpg" >
            <img class="imgpeq" @click="ampliarImg('img4')" id="img4" src="../assets/pizza4.jpg" >
        </div>
      </div>
      <div id="datos">
          <h2>Pizza <span id="fouringrblue">4 ingredientes</span></h2>
          <h4>18.99€</h4>
          <div id="cantidad" align="center">
              <input type="button" @click="cambiarContador(-1)" class="botones" value="-">
              <input type="number" readonly id="quantity" class="botones" :value="contador" >
              <input type="button" @click="cambiarContador(+1)" class="botones" value="+">
          </div>
        <form action="#">
          <div id="comprar" class="buscador">
              <img id="imagencarrito" src="https://img.icons8.com/metro/50/000000/add-shopping-cart.png"/>
              <input type="submit" id="carritobutton" class="buscador" value="Añadir al carrito">
          </div>
        </form>
          <br><br>
        <video width="400" controls>
            <source src="../assets/pizzavideo.mp4" type="video/mp4">
            Vídeo aquí
        </video>
        <Icon path="{mdiCartArrowDown}" />
      </div>
  </div>
</template>

<script>



export default {
  Name: 'ProductoDatos',
    data () {
        return {
            contador: 1
        }
    },
    methods: {
        cambiarContador(num) {
            this.contador += +num;
            if (!isNaN(this.contador) && (this.contador < 0)) {
              this.contador = 0
            }
        },

        ampliarImg(imgX){
            let newSrc = document.getElementById(imgX).src;
            document.getElementById("imgprincipal").src = newSrc;
        }
    }
}


</script>

<style>
    #main{
        display: flex;
        justify-content: center;
    }

    #datos{
        text-align: left;
    }
    #imagencarrito{
        width: 1.3em;
    }
    .botones{
        width: auto;
        font-size: 1.6em;
        text-align: center;
    }
    .imgpeq{
        width: 120px;
        border: solid rgb(163, 163, 163) 1px;
        margin: 1em;
    }
    #imagenes{
        margin-right: 3em;
        padding: 3em 0em 3em 0em;
    }
    #comprar{
        margin-top: 1em;
        display: flex;
        width: auto;
        justify-content: space-around;
        background-color: lightblue;
        padding: 0.3em 1em;
    }
    #comprar:hover{
        border: solid 0.1em rgb(105, 184, 105);
    }
    #carritobutton{
        border: none;
        background-color: transparent;
    }
    video{
        border: solid 0.5em rgb(105, 184, 105);
    }
    #fouringrblue{
        color: rgb(140, 201, 221);
    }
</style>