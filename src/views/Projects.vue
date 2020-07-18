<template>
  <div id="Projects" class="container-fluid">
    <h3 class="text-center">Projects
      <div>
        <img src="../assets/lie2.png" alt="" width=100>
      </div>
    </h3>
    <div class="row">
  <div class="mb-3 col-lg-4 col-md-4 col-sm-4 col-12" :key="index" v-for="(project,index) in projects">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">{{project.name}}</h5>
        <p class="card-text">{{project.desc}}</p>
        <a target="_blank" :href="project.link" class="btn btn-dark" :class="{'disabled': project.name=='E-Book Store'}"><i :class="{'fas fa-external-link-alt': project.button!='Github','fab fa-github':project.button=='Github'}"></i> {{project.button}}</a>
      </div>
    </div>
  </div>
</div>
  </div>
</template>

<script>
export default {
  name : 'Projects',
  data(){
    return{
      projects:[{
        name : 'Garden Management Studio',
        tehnology : ["HTML","JavaScript","CSS","jQuery","Flask","AWS"],
        desc : "Worked on full-stack development to help an NGO.",
        link : "http://admin.brralliance.org/",
        button : 'Admin console'
      },
      {
        name : 'E-Book Store',
        tehnology : ["HTML","JavaScript","CSS","jQuery","Flask","AWS"],
        desc : "Worked on full-stack development to help an NGO.",
        link : "http://admin.brralliance.org/",
        button : 'Github'
      },
      {
        name : 'Android Messenger Application',
        tehnology : ["HTML","JavaScript","CSS","jQuery","Flask","AWS"],
        desc : "Worked on full-stack development to help an NGO.",
        link : "http://admin.brralliance.org/",
        button : 'Github'
      },
      {
        name : 'Monster-Attack Game',
        tehnology : ["VueJS","HTML","JavaScript","CSS","BootStrap"],
        desc : "Worked on full-stack development to help an NGO.",
        link : "http://admin.brralliance.org/",
        button : 'Github'
      }]
    }
  }
}
</script>

<style scoped>

a:hover{
  color: black;
  background-color: white;
}

</style>

