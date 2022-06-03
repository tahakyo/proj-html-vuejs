<template>
  <section>
    <div class="container">
      <div class="footer-content">
        <div class="first-col">
          <div class="logo">
            <img src="../assets/img/35.png" alt="" />
          </div>
          <div class="small-text">
            It is a long established fact that a reader will be distracted by
            the readable content
          </div>
          <div class="copyright">Copyright @ 2018 <a href="">Softbox</a></div>
        </div>
        <div class="footer-menu" v-for="(item, index) in footerMenu" :key="index">
          <ul>
            <li class="menu-title"><a href="">{{item.title}}</a></li>
            <li class="menu-voice"><a href="">{{item.voice1}}</a></li>
            <li class="menu-voice"><a href="">{{item.voice2}}</a></li>
            <li class="menu-voice"><a href="">{{item.voice3}}</a></li>
            <li class="menu-voice"><a href="">{{item.voice4}}</a></li>
            <li class="menu-voice"><a href="">{{item.voice5}}</a></li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Appfooter",
  props: {
    footerMenu: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
section {
  border-top: 1px solid $border-color02;
  padding: 2rem 0 4rem;
  .footer-content {
    display: flex;
    justify-content: space-around;
    .first-col {
      width: calc(100% / 4);
      .logo {
        width: 100px;
      }
      .small-text {
        font-size: 12px;
        color: $text-color04;
        margin-bottom: 2rem;
      }
      .copyright {
        font-size: 12px;
        color: $text-color04;
      }
      .copyright a {
        font-size: 12px;
        color: $text-color05;
      }
    }
    .footer-menu {
      line-height: 3rem;
      .menu-title {
        font-size: 15px;
        font-weight: 500;
      }
      .menu-voice {
        font-size: 12px;
        color: $text-color04;
      }
      a {
        color: inherit;
      }
    }
  }
}
</style>