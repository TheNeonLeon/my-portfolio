<template>
  <div class="project-wrapper">
      <h1>PROJECTS</h1>
  </div>
</template>

<script>
export default {

}
</script>

<style>
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
</style>