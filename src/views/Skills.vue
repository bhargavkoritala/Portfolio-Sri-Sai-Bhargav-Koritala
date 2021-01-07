<template>
  <div id="Skills" class="container-fluid">
    <h3 class="text-center">Skills
      <div>
        <img src="../assets/lie2.png" alt="" width=100>
      </div></h3>
    
    <div>
        <h4 class="font-weight-bold">Programming</h4>
    </div>
    <div class="row">
      <div :key="key" v-for="(value,key) in programmingSkills" class="mb-3 col-lg-4 col-md-4 col-sm-4 col-6">
        <div class="bg-dark rounded p-3">
        <p>
          <i :class="value.icon"></i>
          {{key}}
        </p>
      <div class="icon">
          <div class="progress border border-secondary">
            <div class="progress-bar bg-info" role="progressbar" aria-valuenow="value" aria-valuemin="0" aria-valuemax="100" :style="{width: value.skillValue+'%'}"></div>
          </div>
      </div>
      </div>
      </div>
      
    </div>
    <div>
        <h4 class="font-weight-bold">Web</h4>
      </div>

        <div class="row">
      <div :key="key" v-for="(value,key) in webSkills" class="mb-3 col-lg-4 col-md-4 col-sm-4 col-6">
        <div class="bg-dark rounded p-3">
        <p>
          <i :class="value.icon"></i>
          <img v-if="key=='jQuery'" src="../assets/jquery.png" alt="" width=15 height=15>
          {{key}}
        </p>
      <div class="icon">
          <div class="progress border border-secondary">
            <div class="progress-bar bg-info" role="progressbar" aria-valuenow="value" aria-valuemin="0" aria-valuemax="100" :style="{width: value.skillValue+'%'}"></div>
          </div>
      </div>
        </div>
      </div>
    </div>

    
    <div>
        <h4 class="font-weight-bold">Frameworks</h4>
      </div>
    <div class="row">
      <div :key="key" v-for="(value,key) in frameworks" class="mb-3 col-lg-4 col-md-4 col-sm-4 col-6">
        <div class="bg-dark rounded p-3">
        <p>
          <i :class="value.icon"></i>
          {{key}}
        </p>
      <div class="icon">
          <div class="progress border border-secondary">
            <div class="progress-bar bg-info" role="progressbar" aria-valuenow="value" aria-valuemin="0" aria-valuemax="100" :style="{width: value.skillValue+'%'}"></div>
          </div>
      </div>
        </div>
      </div>
      
    </div>
    <div>
      <h4 class="font-weight-bold">Databases</h4>
    </div>
    <div class="row">
      <div :key="key" v-for="(value,key) in databases" class="mb-3 col-lg-4 col-md-4 col-sm-4 col-6">
          <div class="bg-dark rounded p-3">
          <p>
            <img v-if="key=='MySQL'" style="filter: gray;-webkit-filter: grayscale(1);filter: grayscale(1);" src="../assets/mysql.svg" alt="" width=15 height=15>
            <img v-if="key=='mongoDB'" style="filter: gray;-webkit-filter: grayscale(1);filter: grayscale(1);" src="../assets/mongo.svg" alt="" width=15 height=15>
            <i :class="value.icon"></i>
            {{key}}
          </p>
      <div class="icon">
          <div class="progress border border-secondary">
            <div class="progress-bar bg-info" role="progressbar" aria-valuenow="value" aria-valuemin="0" aria-valuemax="100" :style="{width: value.skillValue+'%'}"></div>
          </div>
      </div>
          </div>
      </div>
      
    </div>
    <div>
        <h4 class="font-weight-bold">Tools</h4>
      </div>
    <div class="row">
      <div :key="key" v-for="(value,key) in Tools" class="col-lg-4 col-md-4 col-sm-4 col-6">
          <div class="bg-dark p-3 rounded">
            <p>
              <img v-if="key=='Grafana'" style="filter: gray;-webkit-filter: grayscale(1);filter: grayscale(1);" src="../assets/grafana.svg" alt="" width=15 height=15>
              <i :class="value.icon"></i>
              {{key}}
            </p>
            <div class="icon">
              <div class="progress border border-secondary">
                <div class="progress-bar bg-info" role="progressbar" aria-valuenow="value" aria-valuemin="0" aria-valuemax="100" :style="{width: value.skillValue+'%'}"></div>
              </div>
            </div>
          </div>
      </div>
      
    </div>
  </div>
</template>

<script>
export default {
  name : 'Skills',
  computed:{
    programmingSkills(){
      return {
        "Java" : {
          skillValue : 80,
          icon : "fab fa-java",
          type : "Programming"
        },
        "Python" : {
          skillValue : 70,
          icon : "fab fa-python",
          type : "Programming"
        }
      }
    },
    webSkills(){
        return{
          "HTML" : {
            skillValue : 85,
            icon : "fab fa-html5",
            type : "Web"
          },
          "JavaScript" : {
            skillValue : 75,
            icon : "fab fa-js-square",
            type : "Web"
          },
          "NodeJS" : {
            skillValue : 60,
            icon : "fab fa-node-js",
            type : "Web"
          },
          "jQuery" : {
            skillValue : 50,
            icon : "jquery"
          },
          "CSS" : {
            skillValue : 60,
            icon : "fab fa-css3-alt"
          },
          "BootStrap" : {
            skillValue : 85,
            icon : "fab fa-bootstrap"
          }
        }
    },
    frameworks(){
      return{
        "VueJS" : {
          skillValue : 80,
          icon : "fab fa-vuejs"
        },
        "ExpressJS" : {
          skillValue : 60,
          icon : ""
        }
      }
    },
    databases(){
      return{
        "MySQL" : {
          skillValue : 60,
          icon : "mysql"
        },
        "mongoDB" : {
          skillValue : 60,
          icon : "mongo"
        }
      }
    },
    Tools(){
      return{
        "Git" : {
          skillValue : 75,
          icon : "fab fa-git-alt"
        },
        "Grafana" : {
          skillValue : 60,
          icon : "grafana"
        }
      }
    }
  }
}
</script>

<style scoped>

p,i{
  color:white;
}

.progress .progress-bar {
  transition: unset;
}

.jquery{
 background-image: url('../../src/assets/jquery.png');
}
</style>
