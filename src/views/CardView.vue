<template>
    <div class="card">
      <ul class="liste" v-for="langages in langage" :key="langages.id">
        <li>{{ langages.id }} </li>
      </ul>
    </div>
  
</template>
<script>
import { langage } from "@/js/langue";

export default {
    name: 'CardView',
  components: {
  
  },
data: () => ({
  langage: langage,
}),
}
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
  grid-template-areas:"text";
  border-radius: 15px;
  background: #8292e5;
  box-shadow: 5px 5px 15px rgba(0, 0, 0, 0.9);
  font-family: 'Light 300 italic';
  width: 50%;
  text-align: center;
  margin: 30px;
  margin-left: 26%;
}

</style>

