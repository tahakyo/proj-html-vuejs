<template>
  <div id="app">
    <header>
      <AppHeader />
    </header>
    <main>
      <AppMain />
    </main>
    <footer>
      <Appfooter />
    </footer>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import Appfooter from './components/Appfooter.vue';

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    Appfooter
}
}
</script>

<style lang="scss">

</style>
