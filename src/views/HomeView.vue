<template>
  <div class="home">
    <img class="photo" src="@/assets/img/moi.jpg" alt="">
    <h1 class="h1">Je suis Léa Hilaire</h1>

        <p class="p1">Et voici mon Portfolio</p>

      <h3 class="h3"> Actuellement en formation à la CCI, afin d'obtenir le Titre professionnel de Développeur Web Web mobile.</h3>

      <h2 class="h2">En cours d'apprentissage</h2>
     <div class="card">
       <card-view/>
      </div>
  </div>
  
</template>

<script>
// @ is an alias to /src
import { langage } from '@/js/langue'
import CardView from './CardView.vue'


export default {
  name: 'HomeView',
  components: {
    CardView
},
  data:()=>({
    langage:langage,
  })
}
</script>
<style>
*{
     margin: 0;
    box-sizing: border-box;
    font-family: 'Light 300 italic' ;
}
body{
    min-height: 100vh;
    background: linear-gradient(#2b1055,#7597de);
}
.liste{
  list-style: none;
  margin: 20px;
  font-size: 22px;
}
.h1{
  margin-top: 50px;
}
.h3{
  margin-top: 50px;
}
.h2{
  margin-top: 150px;
}
.photo{
  margin-top: 70px;
   height: 290px;
   border-radius: 30% 70% 70% 30% / 30% 30% 70% 70% 

}

</style>
