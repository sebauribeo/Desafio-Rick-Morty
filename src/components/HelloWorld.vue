<template>
  <div class="hello container">
    <header class="mx-auto text-center ">
    <img src="../assets/1200px-Rick_and_Morty.svg.png" alt="Rick and Morty" class="img_fluid">
    </header>
    <div class="row">
    <section class="seccion col-12 col-sm-12 col-md-4 col-lg-3 col-xl-3 text-center" v-for="(personaje, index) in personajes" :key="index">
      <h3>{{personaje.nombre}}</h3>
      <img v-bind:src="personaje.src" class="seccion_img" alt="">
    </section>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      personajes:[
        {nombre: 'Rick Sanchez', src:'https://rickandmortyapi.com/api/character/avatar/1.jpeg'},
        {nombre: 'Morty Smith', src:'https://rickandmortyapi.com/api/character/avatar/2.jpeg'},
        {nombre: 'Summer Smith', src:'https://rickandmortyapi.com/api/character/avatar/3.jpeg'},
        {nombre: 'Beth Smith', src:'https://rickandmortyapi.com/api/character/avatar/4.jpeg'},
        {nombre: 'Jerry Smith', src:'https://rickandmortyapi.com/api/character/avatar/5.jpeg'},
        {nombre: 'Cluster Princess', src:'https://rickandmortyapi.com/api/character/avatar/6.jpeg'},
        {nombre: 'Abradolf Lincler', src:'https://rickandmortyapi.com/api/character/avatar/7.jpeg'},
        {nombre: 'Adjudicator Rick', src:'https://rickandmortyapi.com/api/character/avatar/8.jpeg'},
        {nombre: 'Agency Director', src:'https://rickandmortyapi.com/api/character/avatar/9.jpeg'},
        {nombre: 'Alan Rails', src:'https://rickandmortyapi.com/api/character/avatar/10.jpeg'},
        {nombre: 'Albert Einstein', src:'https://rickandmortyapi.com/api/character/avatar/11.jpeg'},
        {nombre: 'Alexander', src:'https://rickandmortyapi.com/api/character/avatar/12.jpeg'},

      ]
    }
  }
}
</script>

<style>
body {
  margin: 0;
  padding: 0;
  border: 0;
}

.seccion {
margin-top: 30px;

}
.seccion_img {
  width: 200px;
  height: 200px;
  margin: 50px;  
  border-radius: 50%;
  box-shadow: 0 0 20px 0 yellow;
}
.img_fluid {
  padding: 50px;
  width: 300px;
  padding: 0;
  margin: 50px;
}
h3 {
  padding: 5px;
  border-radius: 10px;
  color: white;
  font: 200;
  background: red;
}
</style>
