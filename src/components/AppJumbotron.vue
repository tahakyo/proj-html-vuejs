<template>
  <div class="jumbotron">
    <div class="jumbotron__left">
      <div class="title">The biggest platform for your growth.</div>
      <div class="small-text-jumbotron">
        There are many variations of passages of Lorem Ipsum available, but the
        majority has suffered alteration in some form
      </div>
      <div class="button">
        <a href="#" class="myButton">Read More</a>
      </div>
    </div>
    <div class="jumbotron__right">
      <img src="../assets/img/27-1.png" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "AppJumbotron",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
.jumbotron {
  display: flex;
  width: 100vw;
  background-color: $bg-color02;
  padding: 0 2rem;
  &__left {
    display: flex;
    flex-direction: column;
    width: 45%;
    .title {
      font-size: 3rem;
      margin: 2rem 0;
      line-height: 1.5em;
    }
    .small-text-jumbotron {
      color: $text-color04;
      margin: 2rem 0;
    }
    .button {
      margin: 2rem 0;
    }
  }
  &__right {
    width: 55%;
    img {
      position: relative;
      top: 1.7rem;
      left: 3.3rem;
      width: fit-content;
    }
  }
}
</style>