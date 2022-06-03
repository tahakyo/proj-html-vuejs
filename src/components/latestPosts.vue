<template>
  <section>
    <div class="container">
      <div class="text">
        <div class="title">Latest Posts</div>
        <div class="small-text">
          If you are planning on developing a product landing
        </div>
      </div>
      <div class="cards">
        <div v-for="(item, index) in latestPostsCard" :key="index" class="card">
          <div class="card__img">
            <img :src="require(`../assets/img/${item.thumb}`)" alt="" />
            <div class="card__date">{{ item.date }}</div>
          </div>
          <div class="card__text">
            <div class="large-text">{{ item.title }}</div>
            <div class="small-text">
              {{ item.text }}
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "latestPosts",
  props: {
    latestPostsCard: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
section {
  margin-bottom: 6rem;
  .text {
    text-align: center;
    margin-bottom: 4rem;
    .title {
      font-size: 30px;
      padding-bottom: 1rem;
    }
    .small-text {
      font-size: 12px;
      color: $text-color06;
    }
  }
  .cards {
    display: flex;
    justify-content: space-between;
    .card {
      border: 1px solid lightgrey;
      padding: 8px;
      width: calc(100% / 3 - 2rem);
      margin-right: 1rem;
      &__img {
        position: relative;
      }
      &__date {
        position: absolute;
        top: 0;
        background: white;
        margin: 5px;
        font-size: 13px;
        padding: 2px;
        border: 1px solid $border-color02;
        border-radius: 4px;
      }
      &__text {
        .large-text {
          font-size: 17px;
          font-weight: 500;
          margin: 1rem 0;
        }
        .small-text {
          width: 70%;
          font-size: 12px;
          color: $text-color04;
        }
      }
    }
  }
}
</style>