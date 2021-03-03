<template>
  <div id="app">
    <div data-aos="fade-right" data-aos-duration="1000" id="wrapper">
      <h1 class="name">Hello my name is Leon Listo</h1>
      <h1 class="title-info">I'm a Front-end developer</h1>
      <button class="title-btn"><h2>Know more</h2> </button>
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
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #272342;
  margin-top: 60px;
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
    grid-row: 4 / 4;
}
.title-info{
  grid-column: 2/2;
  grid-row: 5 / 5;
  margin-top: -3%;
  margin-left: -8.5%;
}
.title-btn{
    cursor: pointer;
  grid-column: 2/2;
  grid-row: 6 / 6;
  background-color: white;
  border-style: solid;
  border-color: black;
  margin-right: 55%;
  margin-left: 5%;


}
.title-btn::after{
    cursor: pointer;
  background-color: linear-gradient(#000,#434343);

}

</style>
