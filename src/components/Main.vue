<template>
  <main>
      <div class="wrapper">
         <div class="img-container">
            <div 
            v-for="(item, index) in imgMain" :key="index"
            class="imgBox">

               <img :src="item.thumb" alt="">
               <p>{{item.series}}</p>

            </div>
         </div>
      </div>
  </main>
</template>

<script>
export default {
   // gli si assegna il nome prima di importarlo
   name: "Main",
   props:['imgMain']
}
</script>

<style scoped>

main{
   margin-top: 44px;
   width: 100vw;
   background-color: black;
   padding: 50px 0;
}

main h1{
   color: white;
}

p{
   color: white;
}

.img-container{
   display: flex;
   flex-wrap: wrap;
}

.imgBox{
   width: 15%;
   margin: 0 auto;
   padding-top: 15px;
   padding: 0 5px;
   cursor: pointer;
}
</style>