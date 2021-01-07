<template>
  <div id="Background" class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
            <h3 class="text-center">Education & Experience
      <div>
        <img src="../assets/lie2.png" alt="" width=100>
      </div>
    </h3>
    <ul class="timeline">
      
      <!-- Item 1 -->
      <li>
        <div class="comego direction-l">
          <div class="flag-wrapper">
            <span class="hexa"></span>
            <span class="flag text-info">Atwick Inc.</span>
            <span class="time-wrapper"><span class="time bg-info">August 2020 - December 2020</span></span>
          </div>
          <div class="desc text-center font-italic">Full Stack Engineer Intern</div>
          <div class="desc text-justify font-italic">
            <p>
              Developed a full-stack web application using VueJS for client-side architecture 
              and server-side created using Node and MongoDB and upgraded the app from VueJS 2 to VueJS 3.
            </p>
            <p>
              Designed, developed and implemented a NoSQL database architecture based on the analysis
               of business requirements for a high-volume web application improving data integrity
              and execution efficiency.
            </p>
            <p>
              Responsible for integration of third-party API services for video meetings, scheduling appointments
               and enabling payment options resulting in decrease of system complexity.
            </p>
          </div>
        </div>
      </li>

      <!-- Item 1 -->
      <li>
        <div class="comego direction-r">
          <div class="flag-wrapper">
            <span class="hexa"></span>
            <span class="flag text-info">University at Buffalo - SUNY</span>
            <span class="time-wrapper"><span class="time bg-info">August 2019 - Present</span></span>
          </div>
          <div class="desc text-center font-italic">Masters in Computer 
            Science</div>
          <div class="desc text-justify font-italic">  <strong>Coursework: </strong><p>Algorithm analysis and design, Information Retreival, Data Intensive Computing, Distributed Systems, Object Oriented Analysis Design and Implementation, Data models and Query languages.</p></div>
        </div>
      </li>

      <!-- Item 2 -->
      <li>
        <div class="comego direction-l">
          <div class="flag-wrapper">
            <span class="hexa "></span>
            <span class="flag text-info">Infosys Pvt Ltd.</span>
            <div>
              <span class="time-wrapper"><span class="time bg-info">June 2017 - July 2019</span></span>
            </div>
          </div>
          <div class="desc text-center">
            <span class="align-middle font-italic">Systems Engineer</span>
          </div>
          <div class="desc text-justify font-italic">
            <p>Engineered an email content analysis using JavaMail API, that assess header, body and attachments and derived nature, extent and 
                frequency of a risk that ensured operations \& business continuity management by continuous monitoring of mail.</p>
              <p>
                Recommended and executed a server monitoring to estimate optimum usage of a server by providing insights on server stats using Prometheus metrics and Grafana to visualize the dashboards.
              </p>
              <p>
                Improved the back-end search design element for a fashion website through a usability point of view that involves enabling query caching, using full text searches and query optimization.
              </p>
              <p>
                Contributed in a cross-functional team to build a mini-project, to serve as a teaching aid for interns and trainees.
              </p>
          </div>
        </div>
      </li>

      <!-- Item3 -->
      <li>
        <div class="comego direction-r">
          <div class="flag-wrapper">
            <span class="hexa"></span>
            <span class="flag rounded border-secondary text-info">Vellore Institute of Technology</span>
            <div>
              <span class="time-wrapper"><span class="time bg-info">June 2013 - May 2017</span></span>
            </div>
          </div>
          <div class="desc text-justify font-italic">
            <strong>Coursework: </strong>
            <p>Data Structures and Algorithms, Neural Networks, Computer Architecture</p>
          </div>
        </div>
      </li>
    </ul>
  </div>
  </div>
  </div>
</template>

<style scoped>

header h1{
  text-align: center;
  font-weight: bold;
  margin-top: 0;
}
  
 header p{
   text-align: center;
   margin-bottom: 0;
 }

.mytext{
  text-align: justify !important;
}

.hexa{
  border: 0px;
  float: left;
  text-align: center;
  height: 35px;
  width: 60px;
  font-size: 22px;
  background: #17a2b8;
  color: #17a2b8;
  position: relative;
  margin-top: 15px;
}

.hexa:before{
  content: ""; 
  position: absolute; 
  left: 0; 
  width: 0; 
  height: 0;
  border-bottom: 15px solid #17a2b8;
  border-left: 30px solid transparent;
  border-right: 30px solid transparent;
  top: -15px;
}

.hexa:after{
  content: ""; 
  position: absolute; 
  left: 0; 
  width: 0; 
  height: 0;
  border-left: 30px solid transparent;
  border-right: 30px solid transparent;
  border-top: 15px solid #17a2b8;
  bottom: -15px;
}

.timeline {
  position: relative;
  padding: 0;
  width: 100%;
  margin-top: 20px;
  list-style-type: none;
}

.timeline:before {
  position: absolute;
  left: 50%;
  top: 0;
  content: ' ';
  display: block;
  width: 2px;
  height: 100%;
  margin-left: -1px;
  background: rgb(213,213,213);
  background: -moz-linear-gradient(top, rgba(213,213,213,0) 0%, rgb(213,213,213) 8%, rgb(213,213,213) 92%, rgba(213,213,213,0) 100%);
  background: -webkit-gradient(linear, left top, left bottom, color-stop(0%,rgba(30,87,153,1)), color-stop(100%,rgba(125,185,232,1)));
  background: -webkit-linear-gradient(top, rgba(213,213,213,0) 0%, rgb(213,213,213) 8%, rgb(213,213,213) 92%, rgba(213,213,213,0) 100%);
  background: -o-linear-gradient(top, rgba(213,213,213,0) 0%, rgb(213,213,213) 8%, rgb(213,213,213) 92%, rgba(213,213,213,0) 100%);
  background: -ms-linear-gradient(top, rgba(213,213,213,0) 0%, rgb(213,213,213) 8%, rgb(213,213,213) 92%, rgba(213,213,213,0) 100%);
  background: linear-gradient(to bottom, rgba(213,213,213,0) 0%, rgb(213,213,213) 8%, rgb(213,213,213) 92%, rgba(213,213,213,0) 100%);
  z-index: 5;
}

.timeline li {
  padding: 2em 0;
}

.timeline .hexa{
  width: 16px;
  height: 10px;
  position: absolute;
  background: #17a2b8;
  z-index: 5;
  left: 0;
  right: 0;
  margin-left:auto;
  margin-right:auto;
  top: -30px;
  margin-top: 0;
}

.timeline .hexa:before {
  border-bottom: 4px solid #17a2b8;
  border-left-width: 8px;
  border-right-width: 8px;
  top: -4px;
}

.timeline .hexa:after {
  border-left-width: 8px;
  border-right-width: 8px;
  border-top: 4px solid #17a2b8;
  bottom: -4px;
}

.direction-l,
.direction-r {
  float: none;
  width: 100%;
  text-align: center;
}

.flag-wrapper {
  text-align: center;
  position: relative;
}

.flag {
  position: relative;
  display: block;
  background: rgb(255,255,255);
  font-weight: 600;
  z-index: 15;
  padding: 6px 10px;
  text-align: center;
  border-radius: 5px;
}

.direction-l .flag:after,
.direction-r .flag:after {
  content: "";
  position: absolute;
  left: 50%;
  top: -15px;
  height: 0;
  width: 0;
  margin-left: -8px;
  border: solid transparent;
  border-bottom-color: rgb(255,255,255);
  border-width: 8px;
  pointer-events: none;
}

.direction-l .flag {
  -webkit-box-shadow: -1px 1px 1px rgba(0,0,0,0.15), 0 0 1px rgba(0,0,0,0.15);
  -moz-box-shadow: -1px 1px 1px rgba(0,0,0,0.15), 0 0 1px rgba(0,0,0,0.15);
  box-shadow: -1px 1px 1px rgba(0,0,0,0.15), 0 0 1px rgba(0,0,0,0.15);
}

.direction-r .flag {
  -webkit-box-shadow: 1px 1px 1px rgba(0,0,0,0.15), 0 0 1px rgba(0,0,0,0.15);
  -moz-box-shadow: 1px 1px 1px rgba(0,0,0,0.15), 0 0 1px rgba(0,0,0,0.15);
  box-shadow: 1px 1px 1px rgba(0,0,0,0.15), 0 0 1px rgba(0,0,0,0.15);
}

.time-wrapper {
  display: block;
  position: relative;
  margin: 4px 0 0 0;
  z-index: 14;
  line-height: 1em;
  color: #fff;
}

.direction-l .time-wrapper {
  float: none;
}

.direction-r .time-wrapper {
  float: none;
}

.time {
  background: #333;
  display: inline-block;
  padding: 8px;
}

.desc {
  position: relative;
  margin: 1em 0 0 0;
  padding: 1em;
  background: rgb(254,254,254);
  -webkit-box-shadow: 0 0 1px rgba(0,0,0,0.20);
  -moz-box-shadow: 0 0 1px rgba(0,0,0,0.20);
  box-shadow: 0 0 1px rgba(0,0,0,0.20);
  z-index: 15;
}

.direction-l .desc,
.direction-r .desc {
  position: relative;
  margin: 1em 1em 0 1em;
  padding: 1em;
  z-index: 15;
}

.comego{
    -webkit-animation: fadein 1s; /* Safari, Chrome and Opera > 12.1 */
       -moz-animation: fadein 1s; /* Firefox < 16 */
        -ms-animation: fadein 1s; /* Internet Explorer */
         -o-animation: fadein 1s; /* Opera < 12.1 */
            animation: fadein 1s;
}

@keyframes fadein {
    from { opacity: 0; }
    to   { opacity: 1; }
}

/* Firefox < 16 */
@-moz-keyframes fadein {
    from { opacity: 0; }
    to   { opacity: 1; }
}

/* Safari, Chrome and Opera > 12.1 */
@-webkit-keyframes fadein {
    from { opacity: 0; }
    to   { opacity: 1; }
}

/* Internet Explorer */
@-ms-keyframes fadein {
    from { opacity: 0; }
    to   { opacity: 1; }
}


@media(min-width: 768px){
  .timeline {
    width: 660px;
    margin: 0 auto;
    margin-top: 20px;
  }

  .timeline li:after {
    content: "";
    display: block;
    height: 0;
    clear: both;
    visibility: hidden;
  }
  
  .timeline .hexa {
    left: -28px;
    right: auto;
    top: 8px;
  }

  .timeline .direction-l .hexa {
    left: auto;
    right: -28px;
  }

  .direction-l {
    position: relative;
    width: 310px;
    float: left;
    text-align: right;
  }

  .direction-r {
    position: relative;
    width: 310px;
    float: right;
    text-align: left;
  }

  .flag-wrapper {
    display: inline-block;
  }
  
  .flag {
    font-size: 18px;
  }

  .direction-l .flag:after {
    left: auto;
    right: -16px;
    top: 50%;
    margin-top: -8px;
    border: solid transparent;
    border-left-color: rgb(254,254,254);
    border-width: 8px;
  }

  .direction-r .flag:after {
    top: 50%;
    margin-top: -8px;
    border: solid transparent;
    border-right-color: rgb(254,254,254);
    border-width: 8px;
    left: -8px;
  }

  .time-wrapper {
    display: inline;
    vertical-align: middle;
    margin: 0;
  }

  .direction-l .time-wrapper {
    float: left;
  }

  .direction-r .time-wrapper {
    float: right;
  }

  .time {
    padding: 5px 10px;
  }

  .direction-r .desc {
    margin: 1em 0 0 0.75em;
  }
}

@media(min-width: 992px){
  .timeline {
    width: 800px;
    margin: 0 auto;
    margin-top: 20px;
  }

  .direction-l {
    position: relative;
    width: 380px;
    float: left;
    text-align: right;
  }

  .direction-r {
    position: relative;
    width: 380px;
    float: right;
    text-align: left;
  }
}
</style>

