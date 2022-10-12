<script>
export default{
 data:()=>({
  contador:10,
 }),
 methods:{
  saludar(){
    console.log("Hola 10A | @");
  },
  incrementar() {
    this.contador++;
  },
  decrementar() { 
    this.contador--;
  },
  resetear() {
    this.contador=10;
  },
 }
};
</script>

<template>
  <img src="./assets/logo.svg" alt="[logo VUE]" width="125" height="125">
<div class="container">
  <small>
    <h1>Hola desde VUE.js 3</h1>
  </small>
  

<hr>
<!--lo que esta en dentro de laasa llaves es la variable que podemos ir modificando -->
<h2> Contador {{contador}}</h2>
<button @click="incrementar()">+1</button>
<button @click="decrementar()">-1</button>
<button @click="resetear()">Reset</button>

</div>
</template>

<style scoped>
.container{
  text-align: center;
}
small{
  color: rgb(17, 143, 160);
}
/**para el color del h1 */
h1{
  font-weight: bolder;
  
}

h2{
  font-size: 2.5rem;
}
/**para el cursor sombre el boton  */
button{
  cursor:pointer;
  font-size: 1.5rem;
  margin: 0px 8px;
}

</style>
