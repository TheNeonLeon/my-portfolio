<template>
    <div id="about">
      <h1>ABOUT ME</h1>
      <h4 class="about-text">I'm a passionate Front-end developer who loves converting new ideas and concepts into code.
        I'm a visual person with an eye for good and modern design.
      </h4>
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
#about{
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr 1fr 1fr;
  gap: 0px 0px;
  border-style: solid;
  color: white;
  background-image: linear-gradient(
135deg
,#000,#434343);

}
h1{
  grid-row: 1/1;
  grid-column: 3/3;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.about-text{
  grid-row: 3/3;
  grid-column: 4/4;
}

</style>
