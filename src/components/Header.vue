<template>
  <header>
     <div class="wrapper header">
        <div class="logo-header">
           <!-- logo DC -->
           <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <div class="menu-header">
           <ul>
              <!-- ciclo for per i link del menu -->
              <li v-for="(link, index) in linksList" :key="index">
                 <a :class="{active: link.current}" :href="link.url">{{link.text}}</a>
              </li>
           </ul>
        </div>
     </div>
  </header>
</template>

<script>
export default {
   // gli si assegna il nome prima di importarlo
   name: "Header",
   // aggiungo i dati
   data(){
    return{
      linksList:[
        {
          url:'/',
          text: 'Characters',
          current: false
        },
        {
          url:'/comics',
          text: 'comics',
          current: true
        },
        {
          url:'/movies',
          text: 'movies',
          current: false
        },
        {
          url:'/tv',
          text: 'tv',
          current: false
        },
        {
          url:'/games',
          text: 'games',
          current: false
        },
        {
          url:'/collectibles',
          text: 'collectibles',
          current: false
        },
        {
          url:'/videos',
          text: 'videos',
          current: false
        },
        {
          url:'/fans',
          text: 'fans',
          current: false
        },
        {
          url:'/news',
          text: 'news',
          current: false
        },
        {
          url:'/shop',
          text: 'shop',
          current: false
        }
      ]
    }
   }
}
</script>

<style scoped lang="scss">

@import "../assets/style/vars.scss";

   header{
      height: 80px;
      width: 100vw;
      background-color: white;
   }

   .wrapper.header{
      line-height: 80px;
      display: flex;
      justify-content: space-between;
   }

   .logo-header{
      width: 200px;
   }

   .logo-header img{
      width: 120px;
      height: 80%;
      padding: 25px;
      cursor: pointer;
   }

   .menu-header ul{
      display: flex;
      line-height: 100px;
   }

   li{
      list-style: none;
      padding: 10px;
      border-bottom: 3px solid white;
   }

   li a{
      font-size: 13px;
   }

   li:hover,
   li:active{
      border-bottom: 3px solid #0C7BEB;
      border-color: $primary-color;
   }

   li:hover a,
   li:active a{
      color: $primary-color;
   }

</style>