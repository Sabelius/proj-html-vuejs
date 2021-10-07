<template>
  <div class="container-fluid p-5">
    <div class="row">
      <nav class="d-flex">
        <div class="col-8">
          <a :href="logo.url"><img :src="logo.logoImg" /></a>
        </div>
        <div class="col-4">
        <ul class="d-flex justify-content-between pt-2">
          <li v-for="(element, index) in navElements" :key="index">
            <a :href="element.url" class="text-uppercase">{{ element.text }}</a>
          </li>
          <a :href="navMenuButton.url"><img :src="navMenuButton.button" /></a>
        </ul>
        </div>
      </nav>
    </div>
  </div>
</template>

<script>
import logoimg from "../img/logo-sidearea-1.png";
import navimgbutton from "../assets/svg-1.svg";

export default {
  name: "Header",
  data() {
    return {
      logo: {
        url: "#",
        logoImg: logoimg,
      },

      navElements: [
        {
          url: "#",
          text: "home",
        },
        {
          url: "#",
          text: "pages",
        },
        {
          url: "#",
          text: "portfolio",
        },
        {
          url: "#",
          text: "blog",
        },
        {
          url: "#",
          text: "shop",
        },
        {
          url: "#",
          text: "elements",
        },
      ],

      navMenuButton: {
        url: "#",
        button: navimgbutton,
      },
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

ul {
  list-style-type: none;
}
a {
  text-decoration: none;
  color: $text-color;
  font-weight: bold;
}
a:hover {
  color: $text-color;
  text-decoration: 2px solid underline;
  text-decoration-color: $line-color;
}
</style>