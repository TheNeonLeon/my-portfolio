<template>
  <div class="project-wrapper">
      <h1>PROJECTS</h1>
      <h3 class="meetup">The Meetup Hub</h3>
      <p class="meetup-text">{{info1}}. {{info2}}</p>
      <a target="_blank" href="https://tdd-vue-app.herokuapp.com/#/">
      <button class="live-btn">
        <h3>See more </h3>
      </button>
      </a>
  </div>
</template>

<script>
export default {
 data: () => {
   return{
     info1: 'Built a responsive web app for various events. Worked with javascript, vuejs, vuerouter, HTML, CSS, docker and unit testing with vue test utils and jest',
     info2: 'You can see upcoming events from a static JSON file in a user-friendly way'
   }
 }
}
</script>

<style>
.live-btn{
 cursor: pointer;
 width: 40%;
  height: 45%;
  background-color: white;
  border-style: solid;
  border-color: black;
    transition: 0.8s;
    
}
.live-btn:hover{
background-image: linear-gradient(
135deg
,#000,#434343);  
color: white;}
a{
  grid-row: 4/4;
  grid-column: 2/2;
  text-decoration: none;
  color: black;
}
a:hover{
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
}
</style>