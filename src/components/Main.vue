<template>
  <section>
    <jumbotron />
    <cardOne />
  </section>
</template>

<script>
import jumbotron from "./jumbotron.vue";
import cardOne from "./cardOne.vue";

export default {
  name: "Main",
  components: {
    jumbotron,
    cardOne,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
</style>