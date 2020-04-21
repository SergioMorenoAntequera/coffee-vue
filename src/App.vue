<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <TitleAndImages title="FROM THE BEANS"/>
  </div>
</template>

<script>
import TitleAndImages from './components/TitleAndImages.vue'

export default {
  name: 'App',
  components: {
    TitleAndImages
  }
}
</script>

<style>
#app {
  width: 100%;
  min-height: 100vh;

  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;


  background-color: #F7DFBD;
}
</style>
