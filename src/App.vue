<template>
  <div id="app">
    <MainBody msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import MainBody from './components/Main.vue'

export default {
  name: 'app',
  components: {
    MainBody
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 1280px;
  margin: 0 auto;
}
</style>
