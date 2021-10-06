<template>
  <section class="jumbotron">
    <div class="container-fluid p-5">
      <div class="row">
        <div class="d-flex before col-2 align-items-center">
          <i class="fas fa-chevron-circle-left"></i>
        </div>
        <div class="slider col-3">
          <h1>Devotion that never <strong>ends</strong></h1>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tenetur
            illo cupiditate architecto nostrum ex aut placeat odit accusantium
            ea? Veniam ratione iure voluptates mollitia pariatur ut, distinctio
            alias sapiente minima.
          </p>
          <a href="#" class="text-uppercase">Read More</a>
        </div>
        <div class="d-flex col-5 image-container">
          <img :src="image1" />
          <img :src="image2" />
        </div>
        <div class="d-flex after col-2 align-items-center justify-content-end">
          <i class="fas fa-chevron-circle-right"></i>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import imgslider1 from "../img/h-2-slider-img-15.png";
import imgslider2 from "../img/h-2-slider-img-16.png";

export default {
  name: "jumbotron",
  data() {
    return {
      image1: imgslider1,
      image2: imgslider2,
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.image-container {
  padding-left: 200px;
}
h1 {
  font-size: 50px;
}
img {
  width: 300px;
  height: 300px;
}
.fas {
  font-size: 30px;
  color: $fas-color;
}
a {
  text-decoration: none;
  color: $text-color;
  border: 2px solid $fas-color;
  padding: 5px 10px 5px 10px;
  margin-top: 30px;
}
a:hover {
  color: $text-color;
}
</style>