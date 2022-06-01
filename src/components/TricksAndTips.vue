<template>
  <section class="tricks">
    <div class="tricks__left">
      <div class="first-object">
        <div class="large-text">
          Get tips tricks on how to skyrocket your sales
        </div>
        <div class="small-text">
          Faff about only a quid blower I don't want no agro bleeding chimney
          pot burke tosser cras nice one boot fanny.!
        </div>
      </div>
      <div class="second-object">
        <div class="logo">
          <img src="../assets/img/510.png" alt="logo" />
        </div>
        <div class="text">
          <div class="title">Reporting Analysis</div>
          <div class="small-text">
            It is a long established fact that a reader will be distracted by
            the readable content of a page when looking at its layout.
          </div>
        </div>
      </div>
      <div class="third-object">
        <div class="logo">
          <img src="../assets/img/511.png" alt="logo" />
        </div>
        <div class="text">
          <div class="title">Technical SEO Audit</div>
          <div class="small-text">
            It is a long established fact that a reader will be distracted by
            the readable content of a page when looking at its layout.
          </div>
        </div>
      </div>
    </div>
    <div class="tricks__right">
      <img src="../assets/img/509.jpeg" alt="image" />
    </div>
  </section>
</template>

<script>
export default {
  name: "TricksAndTips",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
.tricks {
  display: flex;
  margin-top: 7rem;
  align-items: center;
  justify-content: space-between;
  &__left {
    width: 45%;
    .first-object {
      margin-bottom: 3rem;
      .large-text {
        font-size: 30px;
        margin-bottom: 1rem;
      }
      .small-text {
        font-size: 12px;
        color: $text-color04;
      }
    }
    .second-object {
      display: flex;
      align-items: center;
      box-shadow: 5px 10px 8px 10px $border-color02;
      margin: 3rem 0;
      .logo img {
        width: 50px;
      }
      .text {
        padding: 10px;
        .title {
          font-size: 20px;
          margin-bottom: 0.5rem;
        }
        .small-text {
          font-size: 12px;
          color: $text-color04;
        }
      }
    }
    .third-object {
      display: flex;
      align-items: center;
      margin-bottom: 0 auto;
      .logo img {
        width: 50px;
      }
      .text {
        padding: 10px;
        .title {
          font-size: 20px;
          margin-bottom: 0.5rem;
        }
        .small-text {
          font-size: 12px;
          color: $text-color04;
        }
      }
    }
  }
}
</style>