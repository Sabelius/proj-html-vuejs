<template>
  <jumbotron />
</template>

<script>
import jumbotron from './jumbotron.vue';

export default {
  name: "Main",
  components:{
      jumbotron,
  }
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

</style>