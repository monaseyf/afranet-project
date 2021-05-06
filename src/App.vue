<template>
  <v-app>
    <Nav/> 
    <v-main>
    <about-us></about-us>
    <slider />
    <Members />
    <Gavahi />
    <Customers/>
    <Footer/> 
    <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>
import Nav from './components/nav.vue'
import AboutUs from './components/AboutUs.vue'
import Slider from './components/Slider.vue'
import Members from './components/Members.vue'
import Gavahi from './components/Gavahi.vue'
import Customers from './components/Customers.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    AboutUs,
    Slider,
    Nav,
    Members,
    Gavahi,
    Customers,
    Footer,
  },
}
</script>

<style>

html {
  -webkit-text-size-adjust: 100%;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
body {
  margin: 0;
  font-family: "Open Sans", sans-serif;
  font-size: 16px;
  line-height: 1.5;
}
.v-application--wrap{
  max-width: none;
}
</style>
