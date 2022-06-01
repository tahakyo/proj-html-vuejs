<template>
  <div>
    <div class="container">
      <section class="online_marketing">
        <OnlineMarketingCard v-for="index in marketingCard" :key="index" />
      </section>
      <section>
        <TricksAndTips />
      </section>
    </div>
    <section>
      <PopularFeatures />
    </section>
  </div>
</template>

<script>
import OnlineMarketingCard from "./OnlineMarketingCard.vue";
import TricksAndTips from "./TricksAndTips.vue";
import PopularFeatures from "./PopularFeatures.vue";
export default {
  name: "AppMain",
  components: { OnlineMarketingCard, TricksAndTips, PopularFeatures },
  data: function () {
    return {
      marketingCard: [
        {
          logo: "",
          title: "",
          text: "",
        },
        {
          logo: "",
          title: "",
          text: "",
        },
        {
          logo: "",
          title: "",
          text: "",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";

.online_marketing {
  margin-top: 7rem;
  display: flex;
}
</style>