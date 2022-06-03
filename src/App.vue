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
      <Appfooter :footerMenu="footerMenu"/>
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
      footerMenu: [
        {
          title: "Menu",
          voice1: "About Us",
          voice2: "Theme",
          voice3: "Features",
          voice4: "Pricing",
          voice5: "Blog",
        },
        {
          title: "About Us",
          voice1: "About Sofbox",
          voice2: "Roadmap",
          voice3: "How it Work",
          voice4: "Team",
          voice5: "News",
        },
        {
          title: "Quick Links",
          voice1: "About Us",
          voice2: "Theme",
          voice3: "Features",
          voice4: "Pricing",
          voice5: "Blog",
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
