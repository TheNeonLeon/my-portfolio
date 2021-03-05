<template>
  <div data-aos="fade-right" data-aos-duration="1000" id="app">
    <div id="wrapper">
      <h1 class="name">Hello my name is Leon Listo</h1>
      <h1 class="title-info">I'm a Front-end developer</h1>
      <span v-scroll-to="'#about'" class="title-btn"><h3 class="
      know-more-text">Know more</h3> </span>
    </div>
      <About />
      <Projects />
  </div>
</template>

<script>
import About from './components/About.vue'
import Projects from './components/Projects.vue'

export default {
  name: 'App',
  components: {
    About,
    Projects
  },
  data: () => {
    return {

    }
  },
  methods: {
   
    }
  }
</script>

<style lang="scss">
@import '/style/variables.scss';
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300&display=swap');
body{
    padding: 0px;
margin: 0px;

}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #272342;
  padding: 0;
margin: 0;
}
#wrapper{
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr;
  gap: 0px 0px;
     animation: fadein 2s; 
     min-height: 100vh;
    height: 100vh;
}

.name{
  grid-column: 2/2;
    grid-row: 3 / 3;
    width: 150%;
}
.title-info{
  grid-column: 2/2;
  grid-row: 4 / 4;
  margin-top: -3%;
  margin-left: -8.5%;
      width: 150%;
}
.title-btn{
    cursor: pointer;
  grid-column: 2/2;
  grid-row: 5 / 5;
  background-color: white;
  border-style: solid;
  border-color: black;
  width: 40%;
  height: 40%;
  margin-left: 5%;
  transition: 0.5s;

}
.title-btn:hover{
    cursor: pointer;
  background-image: linear-gradient(
135deg
,#000,#434343);  
color: white;

}
.know-more-text{
  margin-top: 5%;
}

@media (min-width: 1300px) {
 .title-btn{
    cursor: pointer;
  grid-column: 2/2;
  grid-row: 5 / 5;
  background-color: white;
  border-style: solid;
  border-color: black;
  width: 30%;
  height: 30%;
  margin-left: 10%;
 }
}
@media (min-width: 1600px) {
 .title-btn{
    cursor: pointer;
  grid-column: 2/2;
  grid-row: 5 / 5;
  background-color: white;
  border-style: solid;
  border-color: black;
  width: 30%;
  height: 30%;
  margin-left: 20%;

}
}
</style>
