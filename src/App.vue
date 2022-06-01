<template>
  <div id="app">
    <header>
      <AppHeader :navMenu="navMenu" />
    </header>
    <main>
      <AppJumbotron />
      <AppMain />
    </main>
    <footer>
      <Appfooter />
    </footer>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import Appfooter from "./components/Appfooter.vue";
import AppJumbotron from "./components/AppJumbotron.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppMain,
    Appfooter,
    AppJumbotron,
  },
  data: function () {
    return {
      navMenu: [
        {
          url: "#",
          menu: "Home",
          active: "true",
        },
        {
          url: "#",
          menu: "About Us",
          active: "false",
        },
        {
          url: "#",
          menu: "Feature",
          active: "false",
        },
        {
          url: "#",
          menu: "Testimonials",
          active: "false",
        },
        {
          url: "#",
          menu: "Contact Us",
          active: "false",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./assets/style/common.scss";
@import "./assets/style/variables.scss";
header {
  padding: 0.5rem 0;
}
</style>
