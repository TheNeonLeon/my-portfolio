<template>
    <div id="about">
      <h1>ABOUT ME</h1>
      <h4 class="about-text">I'm a passionate Front-end developer who loves converting new ideas and concepts into code.
        I'm a visual person with an eye for good and modern design.
        <br>
        <span class="resume-btn"><a target="_blank" href="https://docdro.id/YXVHSoQ" class="resume-text" >Resume </a>
        </span>
      </h4>
      <img class="portrait" v-bind:src="require(`../assets/portrait.png`)">
    </div>
</template>

<script>
export default {
  name: 'About',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
p{
  font-family: 'Roboto', sans-serif;
}
#about{
  padding: 0;
  margin: 0;
  box-sizing: content-box;
  width: 100%;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
  grid-template-rows: 0.5fr 0.5fr;
  gap: 0px 35px;
  color: white;
  background-image: linear-gradient(
135deg
,#000,#434343);

}
h1{
  grid-row: 1/1;
  grid-column: 3/3;
}
a{
  position: relative;
  border: 2px solid;
  color: white;
  text-decoration: none;
  padding: 1%;
  top: 10%;
    transition: 0.3s;

  
}
a:hover{
  position: relative;
  border: 2px solid;
  color: black;
  background-color: white;
  text-decoration: none;
  padding: 1%;
  top: 10%;
}
.about-text{
  grid-row: 2/2;
  grid-column: 3/3;
  padding-left: 20%;
   width: 200%;
  height: 100%;
}
.resume-btn{
  grid-row: 2/2;
  grid-column: 3/3;
 cursor: pointer;
}
.portrait{
  position: relative;
  grid-row: 2/2;
  grid-column: 2/2;
  width: 100%;
  height: 100%;
  bottom: 12%;
}

</style>
