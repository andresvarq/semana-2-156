<template>
<div id="app">
    <div class="container-fluid">
        <div class="row justify-content-center mb-5">
          <div class="col mt-5" v-for="(item,index) of team" :key="index">
              <team-card :member="item"> </team-card>
          </div> 
        </div>
    </div>
</div>
</template>

<script>

import TeamCard from './components/TeamCard.vue'

export default {
  name: 'App',
  components:{
    TeamCard
  },
  data(){
    return{
    team:[
    {
      codigo: 1,
      nombre: "Amparo González",
      descripcion: "Ingeniera civil de profesión, docente de corazón, comentarista deportiva de frustración. Hincha del buen fútbol.",
      rol: 'Gestora de contenidos.',
      image: './components/img/Foto-Amparo-Gonzalez-min.jpeg',
    },
    {
      codigo: 2,
      nombre: "Mario De la Pava",
      descripcion: "Cuyabro interesado por la tecnología y el nuevo conocimiento. Biker que tiene como terapia rodar y es apasionado por viajar.",
      rol: 'Web Master',
      image: './components/img/Foto-Mario-De-la-Pava-min.jpeg',
    },
    {
      codigo: 3,
      nombre: "Santiago Muñoz",
      descripcion: "Joven de 27 años, mi mayor pasatiempos es la investigación, charlas grupales, los videojuegos y el deporte, aprendiz de programación.",
      rol: 'Dueño del Proyecto',
      image: './components/img/Foto-Santiago-Muñoz-min.png',
    },
    {
      codigo: 4,
      nombre: "Andrés Felipe Vargas",
      descripcion: "Trasegante por el mundo con una guitarra y una palabra, amante de los idiomas, la música y los deportes, fiel seguidor de la comida callejera.",
      rol: 'Administrador del sitio web',
      image: './components/img/Foto-Andres-Felipe-Vargas-min.jpg',
    },
    ] 
    }
  }
}
</script>

