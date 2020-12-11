<template>
  <div id="app">
    <section-header></section-header>
    <section-servicios></section-servicios>
     <section class="container-fluid" id="news" style="margin-top:10px;">
            <div class="d-flex justify-content-center border border-secondary rounded"><h2>Noticias</h2></div>
            <div class="row justify-content-around">
              <section-noticias></section-noticias>
            </div>
     </section>
    <section class="container-fluid" id="team">
      <div class="d-flex justify-content-center border border-secondary rounded" ><h2>Equipo</h2></div>
        <div class="row justify-content-center mb-5">
          <div class="col mt-5" v-for="(item,index) of team" :key="index">
            <team-card v-bind:member="item"></team-card>
          </div>  
        </div>    
          
    </section>
    <PageFooter></PageFooter>
    
  </div>
</template>

<script>

import SectionHeader from './components/SectionHeader.vue'
import SectionServicios from './components/SectionServicios.vue'
import SectionNoticias from './components/SectionNoticias.vue'
import TeamCard from './components/TeamCard.vue'
import PageFooter from './components/PageFooter.vue'


export default {
  name: 'App',
  components:{
    PageFooter,
    SectionHeader,
    SectionServicios,
    TeamCard,
    SectionNoticias,
  },
  data(){
    return{
       team: [        
        {
          codigo : 1,
          nombre : 'Harol Avendaño Patiño',
          descripcion : 'Preguntarse cuándo los ordenadores podrán pensar es como preguntarse cuándo los submarinos podrán nadar, y funciona con algunos seres humanos',
          rol : 'Developer',
          image : "./HA.jpeg",
        }, 
        {
          codigo : 2,
          nombre : 'Jose Chavarrio Alvarado',
          descripcion : 'La inteligencia consiste no solo en el conocimiento, sino también en la destreza de aplicar los conocimientos en la práctica',
          rol : 'Developer',
          image : './JC.jpeg',
        },          
        {
          codigo : 3,
          nombre : 'Luz Hernández Velásquez',
          descripcion : 'Si no puedes correr, camina, si no puedes caminar, gatea. Sin importar lo que hagas, sigue avanzando hacia adelante',
          rol : 'Developer',
          image : './GH.jpeg',
        },     
        {
          codigo : 4,
          nombre : 'Sebastian Jaramillo Restrepo',
          descripcion : 'Si le das a alguien un programa, lo frustrarás un día. Si le enseñas a programar, lo frustrarás toda la vida, y esto aplica para todos los casos',
          rol : 'Developer',
          image : './SJ.jpeg',
        },     
        {
          codigo : 5,
          nombre : 'Juan Camilo Patiño Gomez',
          descripcion : 'Hazlo muy pero muy simple: tan simple como sea posible, pero no más y encontras el mejor camino para triunfar en cualquier cosa que te propones',
          rol : 'Developer',
          image : './JP.jpeg',
        },                     
      ],    
    };
  }
}
</script>

