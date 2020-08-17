<template>
  <div id="app">
   <router-view></router-view>
  </div>
</template>

<script>

import home from './pages/home.vue'
import Faq from './pages/Faq.vue'
import About from './pages/About.vue'


export default {
  name: 'App',
  pages: {
    home,
      Faq,
      About
  }
}
</script>

<style>
    body {
        margin: 0!important;
    }
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /*text-align: center;*/
  /*color: #2c3e50;*/
  /*margin-top: 60px;*/
    box-sizing: border-box;
    margin: 0;
}
</style>
