<template>
  <main>

      <div class="wrapper">

         <button class="series">
            <h3>
               current series
            </h3>
         </button>

         <div class="img-container">

            <div 
            v-for="(item, index) in imgMain" :key="index"
            class="imgBox">

               <img :src="item.thumb" alt="">
               <p>{{item.series}}</p>

            </div>
         </div>

         <button class="load">
            <h3>
               load more
            </h3>
         </button>

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

<style lang="scss" scoped>


@import "../assets/style/vars.scss";

main{
   width: 100vw;
   background-color: black;
   padding: 80px 0 80px;
}

main h1{
   color: white;
}

p{
   color: white;
   font-size: 15px;
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

main .wrapper{
   position: relative;
}

button{
   position: absolute;
   background-color: $primary-color;
   border: none;
   padding: 10px;
   color: white;
}

.series{
   top: -100px;
   left: 0;
}

.load{
   left: 45%;
}

h3{
   text-transform: uppercase;
}
</style>