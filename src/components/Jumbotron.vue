<template>
  <div class="jumbotron">

  </div>
</template>

<script>
export default {
   // gli si assegna il nome prima di importarlo
   name: "Jumbotron"
}
</script>

<style lang="scss" scoped>

@import "../assets/style/vars.scss";

.jumbotron{
   width: 100vw;
   height: 500px;
   background-image: url("../assets/img/jumbotron.jpg");
   background-size: cover;                     
   background-repeat: no-repeat;
   background-position: center center; 

}
   
</style>