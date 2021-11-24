<template>
   <div class="jumbotron">
      <ul>
         <li v-for="(link, index) in linksList2" :key="index">
            <a :class="{active: link.current}" :href="link.url">{{link.text}}</a>
         </li>
      </ul>
   </div>
</template>

<script>
export default {
   // gli si assegna il nome prima di importarlo
   name: "LowJumbo",
   data(){
    return{
      linksList2:[
        {
          url:'/',
          text: 'digital comics',
          current: false
        },
        {
          url:'/',
          text: 'dc merchandise',
          current: false
        },
        {
          url:'/',
          text: 'subscription',
          current: false
        },
        {
          url:'/',
          text: 'comic shop locator',
          current: false
        },
        {
          url:'/',
          text: 'dc power visa',
          current: false
        },
        
      ]
    }
   }
}
</script>

<style scoped>

   .jumbotron{
      height: 90px;
      width: 100%;
      background: #0C7BEB;
   }
</style>