<template>
  <main>
      <div class="wrapper">
         <h1>SPAZIO PER IL MAIN</h1>
      </div>
  </main>
</template>

<script>
export default {
   // gli si assegna il nome prima di importarlo
   name: "Main"
}
</script>

<style scoped>

main{
   height: calc(100% - 365px - 120px - 80px - 70px);
   margin-top: 44px;
   width: 100vw;
   height: 200px;
   background-color: black;
   line-height: 200px; /* DA ELIMINARE */
}

main h1{
   color: white;
}
</style>