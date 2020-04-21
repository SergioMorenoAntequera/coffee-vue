<template>
  <div class="titleAndImages">
    <div class="titleAndImagesContent">
      
      <!-- title  -->
      <div class="row justify-content-center">
        <div class="title col-6">
          <h1> {{ title }}</h1>
        </div>
      </div>

      <!-- Images -->
      <transition name="animate" 
      enter-active-class="animated fadeInDown"
      leave-active-class="animated fadeOutDown">
          
        <div class="images row justify-content-center">
          <div class="col-7 col-md-4 px-0 px-md-4 bg-primary">
            PRA
          </div>
          <div class="col-7 col-md-4 px-0 px-md-4 bg-secondary">
            PRA
          </div>
          <div class="col-7 col-md-4 px-0 px-md-4 bg-primary">
            PRA
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
  props: ['title'],
  data: () => {
    return {
      // PRARIABLES
    };
  }
};
</script>

<style lang="css" scoped>
.titleAndImages .titleAndImagesContent .title {
  position: relative;
  background-color: #4B423C; 
}
.titleAndImages .titleAndImagesContent .title h1 {
  padding-top: 70px;
  padding-bottom: 100px;
  font-weight: bolder;
  color: #BB9C79;
}
.titleAndImages .titleAndImagesContent .images {
  position: relative;
  top: -100px;
}
</style> 