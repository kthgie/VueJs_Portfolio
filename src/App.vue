<template>
  <div id="app">
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">Contact</router-link>
      
    </nav>
    <router-view/>
  </div>
</template>
<script>

export default {
  name: 'HeaderHeader',
  components: {
    
  }
}


</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;

}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
  padding: 6px 15px;
  color: #fff;
  border-radius: 20px;

}

nav a.router-link-exact-active {
background: #fff;
color: #2b1055;
}
</style>
