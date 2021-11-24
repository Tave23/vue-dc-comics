<template>
  <footer>
     <div class="wrapper bottom-footer">
<!-- bottone sign-up -->
         <div class="footer-btn">
            <a href="#">
               <button>sign-up now!</button>
            </a>
         </div> 
<!-- link social -->
         <div class="footer-social">
            <a href="#">
               <h3>follow us</h3>
            </a>

            <ul>

               <li>
                  <a href="#">
                     <img src="../assets/img/footer-facebook.png" alt="">
                  </a>
               </li>
               <li>
                  <a href="#">
                     <img src="../assets/img/footer-twitter.png" alt="">
                  </a>
               </li>
               <li>
                  <a href="#">
                     <img src="../assets/img/footer-youtube.png" alt="">
                  </a>
               </li>
               <li>
                  <a href="#">
                     <img src="../assets/img/footer-pinterest.png" alt="">
                  </a>
               </li>
               <li>
                  <a href="#">
                     <img src="../assets/img/footer-periscope.png" alt="">
                  </a>
               </li>
               
            </ul>
         </div>  
         
     </div>
  </footer>
</template>

<script>
export default {
   // gli si assegna il nome prima di importarlo
   name: "Footer"
}
</script>

<style lang="scss" scoped>

@import "../assets/style/vars.scss";

   footer{
      height: 90px;
      width: 100vw;
      background-color: #303030;
      position: relative;
      z-index: 999;
      padding-top: 10px;
   }

   .wrapper.bottom-footer{
      line-height: 70px;
      display: flex;
      justify-content: space-between;
   }

   .footer-social{
      display: flex;
   }

   a button{
      padding: 10px 15px;
      background-color: #303030;
      color: white;
      border: 2px solid $primary-color;
      text-transform: uppercase;
      cursor: pointer;
   }

   button:hover{
      color: $primary-color;
      background-color: white;
   }

   h3{
      color: $primary-color;
   }

   ul{
      display: flex;
      margin-left: 25px;
   }

   li{
      margin-top: 10px;
      margin-left: 15px;
   }
   
</style>