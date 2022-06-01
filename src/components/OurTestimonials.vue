<template>
  <section>
    <div class="container">
      <div class="testimonials">
        <div class="testimonials__text">
          <div class="title">Our Testimonials</div>
          <div class="small-text">
            If you are planning on developing a product landing app or website,
            take a look at this beautiful-crafted
          </div>
        </div>
        <div class="cards">
          <div class="card">
            <img src="../assets/img/26.jpeg" alt="" />
            <div class="name">Julia Aann</div>
            <span>- coo sofbox</span>
            <div class="small-text"></div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "OurTestimonials",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
section {
  .testimonials {
    &__text {
      text-align: center;
      .title {
        font-size: 30px;
      }
      .small-text {
        font-size: 12px;
        color: $text-color06;
      }
    }
    .cards {
      .card {
        width: 50%;
        text-align: center;
      }
      .card img {
        width: 50px;
        border-radius: 20px;
      }
    }
  }
}
</style>