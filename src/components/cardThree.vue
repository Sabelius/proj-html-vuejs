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
                <svg width="15" viewBox="0 0 100 100">
                  <circle cx="50" cy="50" r="40" />
                </svg>
              </div>
            </button>
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
.bg-container {
  background-image: url("../img/h-2-background-1.jpg");
  background-position: center;
  background-size: cover;
}
h1 {
  font-size: 50px;
}
button {
  padding: 15px 45px;
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
  left: 80%;
}
button:hover svg {
  fill: $period-news-color;
}
</style>