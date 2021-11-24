<template>
   <div class="bg-link">
      <div class="wrapper linkUtili">

         <div class="first-column">
            <ul>
               <h3>dc comics</h3>
               <li v-for="(link, index) in dcComics" :key="index">
                  <a :href="link.url">{{link.text}}</a>
               </li>
            </ul>

            <ul>
               <h3>shop</h3>
               <li v-for="(link, index) in shop" :key="index.item">
                  <a :href="link.url">{{link.text}}</a>
               </li>
            </ul>
         </div>

         <div class="second-column">

            <ul>
               <h3>DC</h3>
               <li v-for="(link, index) in dc" :key="index">
                  <a :href="link.url">{{link.text}}</a>
               </li>
            </ul>

         </div>

         <div class="third-column">

            <ul>
               <h3>DC</h3>
               <li v-for="(link, index) in sites" :key="index">
                  <a :href="link.url">{{link.text}}</a>
               </li>
            </ul>

         </div>
         
         <div class="logo-dc">
            <img src="../assets/img/dc-logo-bg.png" alt="">
         </div>
      </div>
   </div>
</template>

<script>
export default {
   // gli si assegna il nome prima di importarlo
   name: "UsefulLinks",
   // aggiungo i dati
   data(){
      return{
         dcComics:[
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
            text: 'TV',
            current: false
         },
         {
            url:'/games',
            text: 'games',
            current: false
         },
         {
            url:'/videos',
            text: 'videos',
            current: false
         },
         {
            url:'/news',
            text: 'news',
            current: false
         },
         ],

         shop:[
         {
            url:'/',
            text: 'shop DC',
            current: false
         },
         {
            url:'/shopDcCollectibles',
            text: 'shop DC Collectibles',
            current: true
         }
         ],

         dc:[
         {
            url:'/terms',
            text: 'terms of use',
            current: false
         },
         {
            url:'/privacy',
            text: 'privacy policy (New)',
            current: true
         },
         {
            url:'/ad',
            text: 'ad Choices',
            current: false
         },
         {
            url:'/advertising',
            text: 'advertising',
            current: false
         },
         {
            url:'/jobs',
            text: 'jobs',
            current: false
         },
         {
            url:'/subscriptions',
            text: 'subscriptions',
            current: false
         },
         {
            url:'/workshops',
            text: 'talent workshops',
            current: false
         },
         {
            url:'/certificates',
            text: 'CPSC certificates',
            current: false
         },
         {
            url:'/ratings',
            text: 'ratings',
            current: false
         },
         {
            url:'/help',
            text: 'shop help',
            current: false
         },
         {
            url:'/contact',
            text: 'contact us',
            current: false
         },
         ],

         sites:[
         {
            url:'/DC',
            text: 'DC',
            current: false
         },
         {
            url:'/Magazine',
            text: 'MAD Magazine',
            current: true
         },
         {
            url:'/Kids',
            text: 'DC Kids',
            current: true
         },
         {
            url:'/universe',
            text: 'DC universe',
            current: true
         },
         {
            url:'/power',
            text: 'DC power visa',
            current: true
         }
         ],
      }
   }
}
</script>

<style lang="scss" scoped>

   .bg-link{
      width: 100vw;
      height: 365px;
      background-image: url(../assets/img/footer-bg.jpg);
      background-size: cover;                     
      background-repeat: no-repeat;
      background-position: center center; 
      padding: 20px 0;
   }

   .wrapper.linkUtili{
      display: flex;
   }

   h3{
      color: white;
      margin: 20px 0;
      text-transform: uppercase;
   }

   li a{
      color: gray;
      text-transform: capitalize;
   }

   li a:hover{
      color: white;
   }

   .first-column,
   .second-column,
   .third-column{
      margin-right: 35px;
      width: 15%;
   }

   .logo-dc{
      width: 50%;
      margin-left: 100px;
      position: relative;
   }

   .logo-dc img{
      width: 100%;
      position: absolute;
      top: -50px;
      z-index: 997;
   }

</style>
   
