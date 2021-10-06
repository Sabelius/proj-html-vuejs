<template>
  <section>
    <jumbotron />
    <cardOne />
    <cardTwo />
    <cardThree />
  </section>
</template>

<script>
import jumbotron from "./jumbotron.vue";
import cardOne from "./cardOne.vue";
import cardTwo from "./cardTwo.vue";
import cardThree from "./cardThree.vue";

export default {
  name: "Main",
  components: {
    jumbotron,
    cardOne,
    cardTwo,
    cardThree,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
</style>