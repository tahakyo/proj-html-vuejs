<template>
  <div id="app">
    <header>
      <AppHeader />
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
    AppJumbotron
},
};
</script>

<style lang="scss">
@import "./assets/style/common.scss";
@import "./assets/style/variables.scss";
header {
  padding: .5rem 0;
}

</style>
