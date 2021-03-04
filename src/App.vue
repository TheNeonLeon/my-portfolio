<template>
  <div data-aos="fade-right" data-aos-duration="1000" id="app">
    <div id="wrapper">
      <h1 class="name">Hello my name is Leon Listo</h1>
      <h1 class="title-info">I'm a Front-end developer</h1>
      <span v-scroll-to="'#about'" class="title-btn"><h3 class="
      know-more-text">Know more</h3> </span>
    </div>
      <About />
  </div>
</template>

<script>
import About from './components/About.vue'
export default {
  name: 'App',
  components: {
    About
  },
  data: () => {
    return {

    }
  },
  methods: {
   
    }
  }
</script>

<style>
body{
    padding: 0;
margin: -1%;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #272342;
  margin-top: 60px;
  padding: 0;
margin: 0;
}
#wrapper{
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr;
  gap: 0px 0px;
     animation: fadein 2s; 
}

.name{
  grid-column: 2/2;
    grid-row: 3 / 3;
}
.title-info{
  grid-column: 2/2;
  grid-row: 4 / 4;
  margin-top: -3%;
  margin-left: -8.5%;
}
.title-btn{
    cursor: pointer;
  grid-column: 2/2;
  grid-row: 5 / 5;
  background-color: white;
  border-style: solid;
  border-color: black;
  margin-right: 55%;
  margin-left: 5%;
  width: 40%;
  height: 40%;

}
.title-btn::after{
    cursor: pointer;
  background-color: linear-gradient(#000,#434343);

}
.know-more-text{
  margin-top: 10%;
}
</style>
