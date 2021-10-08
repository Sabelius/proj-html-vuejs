<template>
  <section>
    <div class="card-container d-flex">
      <div class="card" v-for="card in cards" :key="card.id">
        <img :src="card.imgUrl" />
        <div class="text">
          <h3>{{ card.title }}</h3>
          <h4>
            <em>{{ card.subtitle }}</em>
          </h4>
        </div>
        <div
          class="
            arrow-container
            d-flex
            justify-content-center
            align-items-center
            text-white
          "
        >
          <i :class="card.img"></i>
        </div>
        <div
          class="
            arrow-container2
            d-flex
            justify-content-center
            align-items-center
            text-white
          "
        >
          <i :class="card.img"></i>
        </div>
        <div
          class="
            shopimg-container
            d-flex
            justify-content-center
            align-items-center
          "
        >
          <img class="shop-img" :src="card.shopimg" />
        </div>
        <div
          class="
            shopimg-container2
            d-flex
            justify-content-center
            align-items-center
          "
        >
          <img class="shop-img2" :src="card.shopimg2" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import img1 from "../img/h-2-port-img-1.jpg";
import img2 from "../img/h-2-port-img-2.jpg";
import img3 from "../img/h-2-port-img-3.jpg";
import img4 from "../img/h-2-port-img-4.jpg";
import img5 from "../img/h-2-port-img-5.jpg";
import img6 from "../img/h-2-port-img-6.jpg";
import svgimg from "../assets/svg-6.svg";
import svgimg2 from "../assets/svg-7.svg";

export default {
  name: "cardOne",
  data() {
    return {
      cards: [
        {
          imgUrl: img1,
        },
        {
          imgUrl: img2,
        },
        {
          imgUrl: img3,
          shopimg: svgimg,
          shopimg2: svgimg2,
        },
        {
          imgUrl: img4,
          title: "Illustrations of novels",
          subtitle: "Illustration",
        },
        {
          imgUrl: img5,
        },
        {
          imgUrl: img6,
          img: "fas fa-arrow-up",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import url("https://fonts.googleapis.com/css2?family=Courgette&display=swap");

.card-container {
  flex-wrap: wrap;
  width: 100%;
}
.card {
  cursor: pointer;
  width: calc(100% / 3);
}
.text {
  position: absolute;
  top: 40%;
  padding: 30px;
  background-color: $jumbo-button;
  transform: scaleX(0);
  transform-origin: left;
}
.text h4 {
  font-family: "Courgette", cursive;
}
.card:nth-child(4):hover .text {
  transform: scaleX(1);
  transform-origin: left;
  transition: all 0.3s linear;
}
.card:nth-child(6) .arrow-container {
  position: absolute;
  top: 90%;
  left: 94%;
  background-color: $date-news-color;
  width: 30px;
  height: 30px;
  cursor: pointer;
}
.card:nth-child(6) .arrow-container2 {
  position: absolute;
  left: 94%;
  background-color: $date-news-color;
  width: 30px;
  height: 30px;
  cursor: pointer;
}
.fa-arrow-up {
  font-size: 25px;
}
.shop-img {
  width: 15px;
}
.shop-img2 {
  filter: invert(100%) sepia(100%) brightness(200%);
  width: 20px;
}
.card:nth-child(3) .shopimg-container {
  position: absolute;
  left: 95.2%;
  top: 23%;
  width: 30px;
  height: 30px;
  background-color: $jumbo-button;
  cursor: pointer;
}
.card:nth-child(3) .shopimg-container2 {
  position: absolute;
  left: 95.2%;
  top: 18%;
  width: 30px;
  height: 30px;
  background-color: $line-color;
  cursor: pointer;
}
</style>