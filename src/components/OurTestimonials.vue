<template>
  <section>
    <div class="testimonials">
      <div class="testimonials__text">
        <div class="title">Our Testimonials</div>
        <div class="small-text">
          If you are planning on developing a product landing app or website,
          take a look at this beautiful-crafted
        </div>
      </div>
    </div>
    <div class="cards">
      <div v-for="(item, index) in testimonialsCard" :key="index" class="card">
        <img :src="require(`../assets/img/${item.icon}`)" alt="" />
        <div class="text">
          <div class="name">{{item.name}}</div>
          <span> - {{item.profession}}</span>
        </div>
        <div class="small-text">
          {{item.desc}}
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "OurTestimonials",
  props: {
    testimonialsCard: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
section {
  .testimonials {
    background-image: url("../assets/img/15.png");
    background-repeat: no-repeat;
    background-size: 95%;
    background-color: $bg-color02;
    padding-bottom: 4rem;
    &__text {
      text-align: center;
      width: 27%;
      margin: 0 auto;
      padding-bottom: 3rem;
      .title {
        font-size: 30px;
        padding-bottom: 1rem;
      }
      .small-text {
        font-size: 12px;
        color: $text-color06;
      }
    }
  }
  .cards {
    display: flex;
    padding: 0.7rem 17rem;
    margin-bottom: 7rem;
    .card {
      width: 50%;
      text-align: center;
      padding: 1rem;
      margin-right: 2rem;
      border: 0.5px darkgray;
      box-shadow: 0px 5px 5px grey, 0px 10px 0px lightgray,
        0px 15px 0px whitesmoke, 0px 15px 0px whitesmoke;
      .small-text {
        font-size: 12px;
        color: $text-color04;
      }
    }
    .card img {
      width: 50px;
      border-radius: 50px;
    }
    .text {
      display: flex;
      justify-content: center;
      align-items: center;
      margin: 1rem 0;
      .name {
        font-size: 15px;
        font-weight: 500;
      }
    }
    .text span {
      font-size: 15px;
      color: $text-color04;
      margin-left: 5px;
    }
  }
}
</style>