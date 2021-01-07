<template>
  <div id="Projects" class="container-fluid">
    <h3 class="text-center">Projects
      <div>
        <img src="../assets/lie2.png" alt="" width=100>
      </div>
    </h3>
    <div class="row">
  <div class="mb-3 col-lg-4 col-md-4 col-sm-4 col-12" :key="index" v-for="(project,index) in projects">
    <div class="card border-info text-light">
      <div class="card-body  bg-dark">
        <h5 class="card-title">{{project.name}}</h5>
        <p class="card-text text-justify">{{project.desc}}</p>
        <a target="_blank" :href="project.link" class="btn btn-info"><i :class="{'fas fa-external-link-alt': project.button=='Admin Console','fab fa-github':project.button=='Github','fab fa-gitlab':project.button=='Gitlab'}"></i> {{project.button}}</a>
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
        desc : "A gardening managament tool that helps in maintaining the plant and vegetation information like growth & weather, tracking of the tasks, events & timesheets and an in-house message application to help the gardeners chat.",
        link : "http://admin.brralliance.org/",
        button : 'Admin console'
      },
      {
        name : 'E-Book Store',
        tehnology : ["HTML","JavaScript","CSS","jQuery","Flask","AWS"],
        desc : "An online book buying platform where a reader/buyer can choose from a variety of categories. To enhance the user experience, recommendations are provided based on trends, previous purchases or search. A seller can also list a book to sell on the platform.",
        link : "https://gitlab.com/bhargavkoritala/bookworm.com",
        button : 'Gitlab'
      },
      {
        name : 'Android Messenger Application',
        tehnology : ["Java Socket Programming", "Android Processes and Threads"],
        desc : "A messaging app that allows user to unicast, broadcast and multicast messages. The messenger is a simplified version of Amazon dynamo with disributed key-value storage that can handle linearizability and availability during failure",
        link : "https://github.com/bhargavkoritala/Distributed-Systems",
        button : 'Github'
      },
      {
        name : 'Monster-Attack Game',
        tehnology : ["VueJS","HTML","JavaScript","CSS","BootStrap"],
        desc : "A computer-player game, where player and computer can deal with variety of attack and heal powers simultaneously. The game is randomzied to include arbitrariness.",
        link : "https://github.com/bhargavkoritala/Monster-Attack-Game",
        button : 'Github'
      },
      {
        name : 'Math Master',
        tehnology : ["VueJS","HTML","JavaScript","CSS","BootStrap"],
        desc : "Online Math Quiz designed to help improve basic math skills in a fun interactive way. The quiz range covers problems involving basics of addition, subtraction, multiplication and subtraction.",
        link : "https://github.com/bhargavkoritala/SuperQuiz-Game",
        button : 'Github'
      },
      {
        name : 'Stock Trading ',
        tehnology : ["VueJS","HTML","JavaScript","CSS","BootStrap"],
        desc : "A Stock Management portal, that lets any person to manage and review the the stocks that had been bought and shows the current trends of stock prices on real-time basis.",
        link : "https://github.com/bhargavkoritala/Stock-Trading-App",
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

