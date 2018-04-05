<template>
  <div id="app">
    <img src="./assets/logo.png">
    <router-view/>
    <div>
      <h1>{{ title }}</h1>
    </div>
    <ninjas></ninjas>
  </div>
</template>

<script>
import Ninjas from './components/Ninjas.vue'
export default {
  name: 'App',
  components: {'ninjas': Ninjas},
  data: function () {
    return {
      title: 'Your first view file, wooooo!'
    }
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
  margin-top: 60px;
}
  h1 {
    color: purple;
  }
</style>
