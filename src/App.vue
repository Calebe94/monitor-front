<template>
  <div id="app" style="padding: 20px;">
        <link rel="stylesheet" 
        href="https://use.fontawesome.com/releases/v5.2.0/css/all.css" 
        integrity="sha384-hWVjflwFxL6sNzntih27bfxkr27PmbbK/iSvJ+a4+0owXq79v+lsFkW54bOGbiDQ" 
        crossorigin="anonymous">

    <div class="container">
      <NavMenu/>
    </div>
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <router-view/>
      <!-- <a class="waves-effect waves-light btn">Botão</a> -->
  </div>
</template>
<script>
  import NavMenu from '@/components/NavMenu.vue'
  export default {
    name: 'App',
    components: {
      NavMenu
    }
  }
</script>

<style>
  @import "~materialize-css/dist/css/materialize.css";
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }
  #nav {
    padding: 30px;
  }

  #nav a {
    font-weight: bold;
    color: #2c3e50;
  }

  #nav a.router-link-exact-active {
    color: #42b983;
  }
  body{
    background-color: #263238 ;
  }
</style>
