<template>
  <div class="project-wrapper">
      <h1>PROJECTS</h1>
      <h3 class="meetup">The Meetup Hub</h3>
      <p class="meetup-text">{{project1.info1}}. {{project1.info2}}. {{project1.info3}}</p>
      <button class="live-btn">
        <a class="tdd-link" target="_blank" href="https://tdd-vue-app.herokuapp.com/#/">
        <h3 class="see-more">See more </h3>
        </a>
      </button>
      <a target="_blank" class="meetup-img" href="https://tdd-vue-app.herokuapp.com/#/">
      <img class="meetup-img" v-bind:src="require(`../assets/tdd.png`)">
      </a>
  </div>
</template>

<script>
export default {
 data: () => {
   return{
     project1: {
     info1: 'Built a responsive web app for various events. Worked with javascript, vuejs, vuerouter, HTML, CSS, docker and unit testing with vue test utils and jest',
     info2: 'You can see upcoming events from a static JSON file in a user-friendly way',
     info3: 'Data is saved in localStorage'
     }
    }
 }
}
</script>

<style lang="scss">

@import '/style/variables.scss';

.live-btn{
 cursor: pointer;
 width: 30%;
  height: 35%;
  background-color: white;
  border-style: solid;
  border-color: black;
    transition: 0.8s;
      grid-row: 4/4;
  grid-column: 2/2;
  margin-top: -2%;
    
}
 .see-more{
     margin-top: 10%;
 }
.live-btn:hover{
background-image: linear-gradient(
135deg
,#000,#434343);  
color: white;}
.tdd-link{
  grid-row: 4/4;
  grid-column: 2/2;
  text-decoration: none;
  color: black;
  
}
.tdd-link:hover{
  color: white;
}
.live-btn:hover{
    cursor: pointer;
  background-image: linear-gradient(
135deg
,#000,#434343);  
color: white;

}
p{
font-family: 'Roboto', sans-serif;
}

.project-wrapper{
display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr;
  gap: 0px 0px;
     animation: fadein 2s; 
     min-height: 100vh;
    height: 100vh;
}
h1{
  grid-column: 3/3;
}
.meetup{
  grid-column: 2/2;
  grid-row: 2/2;

}
.meetup-text{
  position: relative;
  grid-column: 2/2;
  grid-row: 2/2;
  top: 40%;
  letter-spacing: $letter-spacing;

}
.meetup-img{
  grid-column: 4/4;
  grid-row: 2/2;
  width: 100%;
  height: 100%;
  margin-top: 2.5%;
}
.meetup-img:hover{
  -webkit-transform: scale(1.1);
    -ms-transform: scale(1.1);
    transform: scale(1.1);
    transition:all 0.5s ease;
    

}
</style>