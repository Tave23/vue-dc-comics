<template>
   <div class="jumbotron">
         <ul>
         <li id="digital">
            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
            <a href="#">digital comics</a>
         </li>
         <li id="merch">
            <img src="../assets/img/buy-comics-merchandise.png" alt="">
            <a href="#">dc merchandise</a>
         </li>
         <li id="subscr">
            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
            <a href="#">subscriptions</a>
         </li>
         <li id="shop">
            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
            <a href="#">comic shop locator</a>
         </li>
         <li id="visa">
            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
            <a href="#">dc power visa</a>
         </li>
      </ul>
   </div>
</template>

<script>
export default {
   // gli si assegna il nome prima di importarlo
   name: "LowJumbo",
}
</script>

<style scoped>

   .jumbotron{
      height: 120px;
      width: 100%;
      background: #0C7BEB;
      padding: 40px;
      z-index: 998;
      position: relative;
   }

   .jumbotron ul{
      display: flex;
      justify-content: center;
      align-self: center;
      line-height: 40px;
   }

   .jumbotron ul li{
      padding: 0 20px;
      list-style: none;
      display: flex;
      align-self: center;
   }

   li img{
      width: 35px;
      margin-right: 10px;
      cursor: pointer;
   }

   #shop img{
      width: 30px;
   }

   a{
      color: white;
   }
</style>