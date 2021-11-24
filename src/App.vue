<template>
  <body>
    <Header />
    <Main />
    <LowJumbo />
    <UsefulLinks />
    <Footer />
  </body>
</template>

<script>

import Header from './components/Header.vue';
import Main from './components/Main.vue';
import LowJumbo from './components/LowJumbo.vue';
import UsefulLinks from './components/UsefulLinks.vue';
import Footer from './components/Footer.vue';



export default {
  name: 'App',
  components: {
    Header,
    Main,
    LowJumbo,
    UsefulLinks,
    Footer
  }
}
</script>

<style>

@import "./assets/style/generals.scss";

</style>
