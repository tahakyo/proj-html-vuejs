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
        <div class="card">
          <div class="title">Customized Invoices</div>
          <div class="icon"><img src="../assets/img/icon7.png" alt="" /></div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "PopularFeatures",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
section {
  background-image: url("../assets/img/14.png");
  background-repeat: no-repeat;
  background-position-x: -400px;
  background-size: 40%;
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
        width: 80%;
      }
    }
  }
  .cards {
    .card {
      width: 25%;
      box-shadow: 0px 1px 20px 5px lightgrey;
      padding: 5px;
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