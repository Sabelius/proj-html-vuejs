<template>
  <section>
    <jumbotron />
    <cardOne />
    <cardTwo />
  </section>
</template>

<script>
import jumbotron from "./jumbotron.vue";
import cardOne from "./cardOne.vue";
import cardTwo from "./cardTwo.vue";

export default {
  name: "Main",
  components: {
    jumbotron,
    cardOne,
    cardTwo,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
</style>