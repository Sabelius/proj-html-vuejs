<template>
  <section>
    <div class="container-fluid">
      <div class="row">
        <div class="col-12">
          <div class="container">
            <div class="row">
              <div class="col-12 d-flex justify-content-center pt-5 pb-5">
                <h1>Working <strong>process</strong></h1>
              </div>
            </div>
            <div class="row">
              <div class="svg-bg d-flex justify-content-between">
                <div
                  class="process-container col-2 pt-1"
                  v-for="element in elements"
                  :key="element.id"
                >
                  <div class="d-flex justify-content-center">
                    <div
                      class="
                        element-img
                        d-flex
                        align-items-center
                        justify-content-center
                      "
                    >
                      <i :class="element.img"></i>
                    </div>
                  </div>
                  <h3 class="text-center pt-3"><strong>{{ element.title }}</strong></h3>
                  <p class="text-center">{{ element.subtitle }}</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-12 d-flex justify-content-end">
          <div
            class="
              arrow-container
              d-flex
              justify-content-center
              align-items-center
              text-white
            "
          >
            <i class="fas fa-arrow-up"></i>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "cardTwo",
  data() {
    return {
      elements: [
        {
          img: "fas fa-lightbulb",
          title: "First theres an idea",
          subtitle:
            "Lorem ipsum dolor sit, conetu adipisc sed be et ore aliqua pleasure itself.",
        },
        {
          img: "far fa-comment",
          title: "Then we talk about",
          subtitle:
            "Lorem ipsum dolor sit, conetu adipisc sed be et ore aliqua pleasure itself.",
        },
        {
          img: "fas fa-cloud",
          title: "And we think about",
          subtitle:
            "Lorem ipsum dolor sit, conetu adipisc sed be et ore aliqua pleasure itself.",
        },
        {
          img: "fas fa-pen-nib",
          title: "So we draw along",
          subtitle:
            "Lorem ipsum dolor sit, conetu adipisc sed be et ore aliqua pleasure itself.",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import url("https://fonts.googleapis.com/css2?family=Courgette&display=swap");

h1 strong {
  font-family: "Courgette", cursive;
}
.svg-bg {
  background-image: url("../assets/svg-3.svg");
  background-position: top;
  background-repeat: no-repeat;
  background-size: 75%;
}
.element-img {
  background-color: $process-icon-bg;
  border-radius: 100%;
  width: 100px;
  height: 100px;
}
i {
  font-size: 35px;
}
.process-container:nth-child(1) i {
  color: $process-icon1;
}
.process-container:nth-child(2) i {
  color: $process-icon2;
}
.process-container:nth-child(3) i {
  color: $process-icon3;
}
.process-container:nth-child(4) i {
  color: $process-icon4;
}
h3 {
  font-size: 20px;
}
p {
  font-size: 11px;
  color: $subtitle-color;
}
.arrow-container {
  background-color: $date-news-color;
  width: 30px;
  height: 30px;
  cursor: pointer;
}
.fa-arrow-up {
  font-size: 25px;
}
</style>