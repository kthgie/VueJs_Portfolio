<template>
<div>
  <div class="card" v-for="(langage,idx) in langages" :key="idx">
    <ul class="liste" >
      <li>{{ langage.id }}</li>
       <img :src="imgUrl(langage.images)" alt=""/>


    </ul>
   
  </div>
</div>
</template>
<script>
import { langages } from "@/js/langues.js";

export default {
  name: "CardView",
  components: {},
  data: () => ({
    langages
  }),
  methods: {
    imgUrl(link){
      return require(`@/assets/img/` + link + `.png`)
    }
  }
  
};
</script>

<style scoped>
body {
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}
.card {
  display: grid;
  grid-template-areas: "text";
  border-radius: 15px;
  background: #8292e5;
  box-shadow: 5px 5px 15px rgba(0, 0, 0, 0.9);
  font-family: "Light 300 italic";
  width: 50%;
  text-align: center;
  margin: 30px;
  margin-left: 26%;
}
img{
  width: 10%
}
</style>

