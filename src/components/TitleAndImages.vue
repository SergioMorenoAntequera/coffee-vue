<template>
  <div class="titleAndImages">
    <div class="titleAndImagesContent">
      <div class="title">
        <h1> {{ title }}</h1>
      </div>
      <div class="images"></div>
    </div>
  </div>
</template>

<script>
// import image from "./assets/logo.png";

export default {
  name: "TitleAndImagesContent",
  props: ['title'],
  data: function() {
    return {
      //image: image
    };
  }
};
</script>

<style lang="css" scoped>
.titleAndImages {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
  position: relative;
  display: flex;
  justify-content: center;
  min-height: 500px;
  min-width: 100%;
}
.titleAndImages .titleAndImagesContent {
  position: relative;
  display: flex;
  justify-content: center;
  width: 90%;
}
.titleAndImages .titleAndImagesContent .title {
  position: relative;
  width: 45%;
  height: 50px;

  text-align: center;
  background-color: #4B423C;
  padding: 65px 30px 130px 30px;
}
.titleAndImages .titleAndImagesContent .title h1 {
  display: inline-block;
  font-weight: bolder;
  color: #BB9C79;
}
.titleAndImages .titleAndImagesContent .images {
  position: absolute;
  top: 120px;
  width: 100%;
  height: 50px;
  background-color: red;
}
</style> 