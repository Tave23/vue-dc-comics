<template>
  <body>
    <Header />
    <Main />
    <LowJumbo />
    <Footer />
  </body>
</template>

<script>

import Header from './components/Header.vue';
import Main from './components/Main.vue';
import LowJumbo from './components/LowJumbo.vue';
import Footer from './components/Footer.vue';



export default {
  name: 'App',
  components: {
    Header,
    Main,
    LowJumbo,
    Footer
  }
}
</script>

<style>

@import "./assets/style/generals.scss";

</style>
