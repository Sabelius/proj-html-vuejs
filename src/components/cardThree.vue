<template>
  <section>
    <div class="container-fluid">
      <div class="row pt-5 pb-5">
        <div class="col-12 text-center pt-5 bg-container">
          <h1 class="pt-5">
            Want to work with us? Send us <strong>a message!</strong>
          </h1>
          <p class="pt-2">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore. Ut enim ad minim
            veniam, quis nostrud exercitation <br />
            ullamco laboris nisi ut aliquip ex ea commo.
          </p>
          <div class="pt-5 pb-5 button-container d-flex justify-content-center">
            <button type="button" class="text-uppercase fw-bold">
              contact
              <div>
                <svg width="20" viewBox="0 0 100 100">
                  <circle cx="50" cy="50" r="40" />
                </svg>
              </div>
            </button>
          </div>
        </div>
      </div>
      <div class="row">
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
  name: "cardThree",
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import url("https://fonts.googleapis.com/css2?family=Courgette&display=swap");

.bg-container {
  background-image: url("../img/h-2-background-1.jpg");
  background-position: center;
  background-size: cover;
}
h1 {
  font-size: 50px;
}
strong {
  font-family: "Courgette", cursive;
}
button {
  padding: 10px 45px;
  background-color: $contact-button;
  border: none;
  position: relative;
}
button:hover {
  color: $jumbo-button;
  background-color: $fas-color;
  transition: all 0.3s linear;
}
svg {
  position: absolute;
  fill: none;
  pointer-events: none;
  top: 59%;
  left: 80%;
}
button:hover svg {
  fill: $period-news-color;
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