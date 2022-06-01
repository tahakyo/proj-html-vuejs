<template>
  <section>
    <div class="container">
      <div class="features">
        <div class="text">
          <div class="text__title">
            Popular features that your business needs
          </div>
          <div class="text__small">
            Faff about only a quid blower I don't want no agro bleeding chimney
            pot burke tosser cras nice one boot fanny!
          </div>
        </div>
        <div class="button">
          <div class="myButton">Explore More features</div>
        </div>
      </div>
      <div class="cards">
        <div v-for="(item, index) in featuresCard" :key="index" class="card">
          <div class="title">{{item.title}}</div>
          <div class="icon"><img :src="require(`../assets/img/${item.icon}`)" alt="" /></div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "PopularFeatures",
  props: {
    featuresCard: Array
  }
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
section {
  background-image: url("../assets/img/14.png");
  background-repeat: no-repeat;
  background-position-x: -300px;
  background-size: 30%;
  .features {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 4rem 0 2rem;
    .text {
      width: 75%;
      &__title {
        font-size: 30px;
        margin-bottom: 1rem;
      }
      &__small {
        font-size: 12px;
        color: $text-color04;
        width: 50%;
      }
    }
    .button {
      padding-right: 3rem;
    }
  }
  .cards {
    display: flex;
    flex-wrap: wrap;
    padding-bottom: 5rem;
    .card {
      width: calc(100% / 4 - 1rem);
      box-shadow: 0px 1px 20px 5px lightgrey;
      padding: 5px;
      margin: 0 1rem 1rem 0;
      .title {
        font-size: 15px;
        font-weight: 400;
        margin-bottom: 1rem;
      }
      .icon {
        width: 25%;
      }
      .icon img {
        width: 50px;
      }
    }
  }
}
</style>