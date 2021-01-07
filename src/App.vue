<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-light text-info">
  <router-link class="navbar-brand" to="/" active-class="active" exact>
      <img src="../public/bklogo.jpg" width="30" height="30" class="d-inline-block align-top" alt="" loading="lazy">
      Sri Sai Bhargav Koritala
    </router-link>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>

  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav ml-auto mt-1">
      <router-link tag="li" to="/background" class="nav-item mx-3"><a data-toggle="collapse" data-target=".navbar-collapse.show" class="nav-link">Background</a></router-link>
      <router-link tag="li" to="/skills" class="nav-item mx-3"><a data-toggle="collapse" data-target=".navbar-collapse.show" class="nav-link">Skills</a></router-link>
      <!-- <router-link tag="li" to="/experience" class="nav-item mx-3"><a class="nav-link">Experience </a></router-link> -->
      <router-link tag="li" to="/projects" class="nav-item mx-3"><a data-toggle="collapse" data-target=".navbar-collapse.show" class="nav-link">Projects</a></router-link>
    </ul>
  </div>
</nav>
    <router-view/>
    <Footer></Footer>
  </div>
</template>

<script>

import Footer from './components/Footer';

export default {
  name: 'App',
  components : {
    Footer
  }
}
</script>


<style>



#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

nav li a  {
  color: #17a2b8;
}

 nav a:hover,
 nav a.router-link-active,
 nav a.router-link-exact-active {
     color: #17a2b8 !important;
 }

.router-link-exact-active a{
  color: #17a2b8 !important;
}

body{
  height:100vh;
}

.skill-unit .bar .progress { background: #000; }
.skill-unit .bar .progress span { color: #000; background: 0vmax}
</style>
