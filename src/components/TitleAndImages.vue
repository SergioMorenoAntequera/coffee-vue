<template>
  <div class="titleAndImages">
    <div class="titleAndImagesContent">
      
      <!-- title  -->
      <div class="row justify-content-center">
        <div @click="animated = !animated" class="title col-6">
          <h1> {{ title }}</h1>
        </div>
      </div>
      
      <!-- Images -->

        <transition name="animate" 
        enter-active-class="animated fadeInDown"
        leave-active-class="animated fadeOutDown">

          <div v-if="animated" class="images row justify-content-center">
            <div class="col-6 col-md-3">
              <img class="img-fluid" :src="img1" alt="Coffe beans picture">
            </div>
            <div class="col-6 col-md-3 px-1">
              <img class="img-fluid" :src="img2" alt="Coffe beans picture">
            </div>
            <div class="d-none d-md-block col-md-3">
              <img class="img-fluid" :src="img3" alt="Coffe beans picture">
            </div>
          </div>
        </transition>
      
    </div>
  </div>
</template>

<script>
// import image from "./assets/logo.png";
export default {
  name: "TitleAndImagesContent",
  props: ['title', "img1", "img2", "img3"],
  data: () => {
    return {
      animated: false,
      // PRARIABLES
    };
  }
};
</script>

<style lang="css" scoped>
.titleAndImages {
  overflow: hidden;
  min-height: 100vh;
}
.titleAndImagesContent{
  overflow: hidden;
}
.titleAndImages .titleAndImagesContent .title {
  position: relative;
  background-color: #4B423C; 
}
.titleAndImages .titleAndImagesContent .title h1 {
  padding-top: 50px;
  padding-bottom: 120px;
  font-weight: bolder;
  color: #BB9C79;
}
.titleAndImages .titleAndImagesContent .images {
  position: relative;
  top: -80px;
  margin-bottom: -80px;
}
.titleAndImages .titleAndImagesContent .images img {
  height: 400px;
  width: 80%;
}
</style> 