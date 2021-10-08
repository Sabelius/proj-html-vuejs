<template>
  <section>
    <div class="container">
      <div class="row d-flex pt-5">
        <div
          class="news-container col-4"
          v-for="news in newsSection"
          :key="news.id"
        >
          <div class="date-container">
            <div class="date d-flex justify-content-center">
              <h2 class="pt-1">{{ news.date }}</h2>
            </div>
            <div
              class="period d-flex justify-content-center align-items-center"
            >
              <h6>{{ news.dayMonth }}</h6>
            </div>
          </div>
          <div class="news-image">
            <a :href="news.url"><img :src="news.img" /></a>
          </div>
          <div class="title pt-3 pb-5">
            <h2>{{ news.title }}</h2>
            <h6>
              <em>{{ news.signature }}</em>
            </h6>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import image from "../img/h-2-blog-img-1.jpg";
import image2 from "../img/h-2-blog-img-2.jpg";
import image3 from "../img/h-2-blog-img-3.jpg";

export default {
  name: "cardFour",
  data() {
    return {
      newsSection: [
        {
          date: "07",
          dayMonth: "May '19",
          url: "#",
          img: image,
          title: "This way, loves: a detailed guide through new design",
          signature: "by Emily Fields",
        },
        {
          date: "07",
          dayMonth: "May '19",
          url: "#",
          img: image2,
          title: "I try to give people a different way to looking art",
          signature: "by Emily Fields",
        },
        {
          date: "07",
          dayMonth: "May '19",
          url: "#",
          img: image3,
          title: "Introduce Richard Laperrière of those amazing features",
          signature: "by Emily Fields",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import url("https://fonts.googleapis.com/css2?family=Courgette&display=swap");

.news-container {
  position: relative;
}
img {
  width: 420px;
}
.date-container {
  position: absolute;
  top: -20px;
  left: 20px;
}
.date {
  background-color: $date-news-color;
  width: 60px;
  height: 30px;
}
.date h2 {
  font-size: 20px;
}
.period {
  width: 60px;
  height: 30px;
  background-color: $period-news-color;
  clip-path: polygon(0 0, 100% 0, 100% 100%, 50% 70%, 0 100%);
}
.period h6 {
  font-size: 15px;
}
.title h2 {
  font-size: 20px;
}
.title h6 {
  font-size: 15px;
  font-family: "Courgette", cursive;
}
</style>