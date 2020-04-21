<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <TitleAndImages class="title-images" title="FROM THE BEANS"
    img1="https://i.imgur.com/O7RNwIh.jpg" 
    img2="https://i.imgur.com/95GQqUA.jpg" 
    img3="https://i.imgur.com/LL7fpdN.jpg"/>
    
    <TitleAndImages class="title-images" title="TO THE CUP"
    img1="https://i.imgur.com/4S8CzAc.jpg" 
    img2="https://i.imgur.com/qZTOH0D.jpg" 
    img3="https://i.imgur.com/oaMmxLg.jpg"/>
  </div>
</template>

<script>
import TitleAndImages from './components/TitleAndImages.vue'

export default {
  name: 'App',
  components: {
    TitleAndImages
  },
  data: () => {
    return {
      // 
    }
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
.title-images {
  position: relative;
}
</style>
