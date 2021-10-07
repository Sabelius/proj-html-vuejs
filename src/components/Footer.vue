<template>
  <section>
    <div class="container-fluid pt-5">
      <div class="row">
        <div class="col-12">
          <div class="container pt-4 pb-5">
            <div class="row">
              <div class="logo col-3" v-for="logo in footerLogo" :key="logo.id">
                <a :href="logo.url"><img :src="logo.footerLogo" /></a>
                <h6 class="pt-2">{{ logo.slogan }}</h6>
              </div>
              <div
                v-for="contact in footerContacts"
                :key="contact.id"
                class="col-3 pt-3 contact-us"
              >
                <h6>{{ contact.email }}</h6>
                <h6>{{ contact.number }}</h6>
              </div>
              <div class="home col-3 pt-3" v-for="position in footerPosition"
                :key="position.id">
                <h6>{{ position.address }}</h6>
                <h6>{{ position.position }}</h6>
              </div>
              <div class="col-3 pt-3">
                <h6 class="text-center">Stay in touch with us</h6>
                <ul class="d-flex">
                  <li v-for="social in footerSocials" :key="social.id">
                    <a :href="social.urlWeb" target="blank"
                      ><i class="fab" :class="social.symbol"></i
                    ></a>
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import logo from "../img/logo-sidearea-1.png";

export default {
  name: "Footer",
  data() {
    return {
      footerLogo: [
        { url: "#", footerLogo: logo, slogan: "Let's Get Creative" },
      ],
      footerContacts: [
        {
          email: "maree.qode@gmail.com",
          number: "+44645 321 789",
        },
      ],
      footerPosition: [
        {
          address: "Avenue d'Auderghem 10",
          position: "1040 Brussels, Belgium",
        },
      ],
      footerSocials: [
        {
          urlWeb: "https://twitter.com/",
          symbol: "fa-twitter",
        },
        {
          urlWeb: "https://www.pinterest.com/",
          symbol: "fa-pinterest-p",
        },
        {
          urlWeb: "https://www.facebook.com/",
          symbol: "fa-facebook-f",
        },
        {
          urlWeb: "https://www.linkedin.com/",
          symbol: "fa-linkedin-in",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.container-fluid {
  background-color: $date-news-color;
}
ul {
  list-style: none;
}
li {
  padding-left: 38px;
}
a {
  color: $text-color;
}
a:hover{
  color: $text-color;
}
</style>