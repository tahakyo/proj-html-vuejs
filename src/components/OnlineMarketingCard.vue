<template>
  <div class="container">
    <div class="online-marketing">
      <div v-for="(element, index) in marketingCard" :key="index" class="card">
        <div class="card__head">
          <img
            class="logo"
            :src="require(`../assets/img/${element.logo}`)"
            alt="logo"
          />
          <div class="text">
            <div class="title">{{ element.title }}</div>
            <div class="small_text">
              {{ element.text }}
            </div>
          </div>
        </div>
        <ul>
          <li><i class="fas fa-check"></i>seo</li>
          <li><i class="fas fa-check"></i>sem</li>
          <li><i class="fas fa-check"></i>Website Strategy</li>
          <li><i class="fas fa-check"></i>social management</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "OnlineMarketingCard",
  props: {
    marketingCard: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
.online-marketing {
  display: flex;
  margin-top: 7rem;
  .card {
    padding: 1rem;
    &__head {
      display: flex;
      align-items: center;
      .logo {
        width: 80px;
      }
      .text {
        .title {
          font-size: 20px;
          margin-bottom: 1rem;
        }
        .small_text {
          font-size: 12px;
          color: $text-color04;
          width: 80%;
        }
      }
    }
    ul {
      margin-top: 1rem;
      margin-left: 4rem;
      line-height: 30px;
      li i {
        color: #377dff;
        padding: 0 12px;
        font-size: 14px;
      }
      li {
        text-transform: uppercase;
        font-size: 10px;
        font-weight: bold;
      }
    }
  }
}
</style>