<template>
  <section>
    <div class="container-fluid">
      <div class="card-container d-flex">
        <div class="card" v-for="card in cards" :key="card.id">
          <img :src="card.imgUrl" />
          <div class="text">
          <h3>{{ card.title}}</h3>
          <h4><em>{{ card.subtitle}}</em></h4>
          </div>
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
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.card-container {
  flex-wrap: wrap;
  width: 100%;
}
.card {
  cursor: pointer;
  width: calc(100% / 3);
}
.text{
  position: absolute;
  top: 40%;
  padding: 30px;
  background-color: $jumbo-button;
  transform: scaleX(0);
  transform-origin: left;
}
.card:nth-child(4):hover .text{
  transform: scaleX(1);
  transform-origin: left;
  transition: all 0.3s linear;
}
</style>