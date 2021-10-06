<template>
  <section>
    <div class="container-fluid">
      <div class="row">
        <div class="col-12 text-center pt-5 bg-container">
          <h1 class="pt-5">Want to work with us? Send us <strong>a message!</strong></h1>
          <p class="pt-2">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore. Ut enim ad minim
            veniam, quis nostrud exercitation <br> ullamco laboris nisi ut aliquip ex
            ea commo.
          </p>
          <div class="pt-5 pb-5">
          <button type="button" class="text-uppercase fw-bold">contact</button>
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
.bg-container{
    background-image: url("../img/h-2-background-1.jpg");
}
h1{
    font-size: 50px;
}
button{
    padding: 10px 40px;
    background-color: $contact-button;
    border: none;
}

</style>