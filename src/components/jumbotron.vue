<template>
  <section class="jumbotron">
    <div class="container-fluid p-5">
      <div class="row">
        <div class="d-flex before col-2 align-items-center">
          <i class="fas fa-chevron-circle-left arrow"></i>
        </div>
        <div class="slider col-4">
          <h1>Devotion that never <strong>ends</strong></h1>
          <p>
            Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet,
            consectetur, adipisci velit, sed quia non numquam eius modi.
          </p>
          <button type="button" class="text-uppercase fw-bold">
            read more
          </button>
        </div>
        <div class="d-flex col-4 image-container">
          <img :src="image3" class="small" />
          <img :src="image7" class="small sm-seven" />
          <img :src="image6" class="small sm-six" />
          <img :src="image1" />
          <img :src="image2" />
          <img :src="image4" class="small sm-four" />
          <img :src="image5" class="small" />
          <img :src="image8" class="small sm-eight" />
        </div>
        <div class="d-flex after col-2 align-items-center justify-content-end">
          <i class="fas fa-chevron-circle-right arrow"></i>
        </div>
        <div class="dots d-flex col-12 justify-content-center pt-5">
          <i class="fas fa-circle"></i>
          <i class="fas fa-circle"></i>
          <i class="fas fa-circle"></i>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import imgslider1 from "../img/h-2-slider-img-15.png";
import imgslider2 from "../img/h-2-slider-img-16.png";
import imgslider3 from "../img/short-slider-rev-1-img-2.png";
import imgslider4 from "../img/short-slider-rev-1-img-6.png";
import imgslider5 from "../img/short-slider-rev-1-img-7.png";
import imgslider6 from "../img/short-slider-rev-1-img-8.png";
import imgslider7 from "../img/short-slider-rev-1-img-10.png";
import imgslider8 from "../img/h-2-slider-img-17.png";

export default {
  name: "jumbotron",
  data() {
    return {
      image1: imgslider1,
      image2: imgslider2,
      image3: imgslider3,
      image4: imgslider4,
      image5: imgslider5,
      image6: imgslider6,
      image7: imgslider7,
      image8: imgslider8,
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import url("https://fonts.googleapis.com/css2?family=Courgette&display=swap");

.image-container {
  padding-left: 50px;
}
h1 {
  font-size: 70px;
}
strong {
  font-family: "Courgette", cursive;
}
img {
  width: 300px;
  height: 300px;
}
.small {
  width: 50px;
  height: 50px;
}
.sm-seven {
  margin-top: 150px;
}
.sm-six {
  margin-top: 250px;
}
.sm-four {
  margin-top: 120px;
}
.sm-eight {
  margin-top: 250px;
}
.arrow {
  font-size: 30px;
  color: $fas-color;
}
button {
  background-color: $jumbo-button;
  border: 2px solid $fas-color;
  padding: 10px 40px;
  margin-top: 30px;
}
a:hover {
  color: $text-color;
}
.fa-circle {
  padding-left: 20px;
  font-size: 10px;
  color: $fas-color;
}
</style>