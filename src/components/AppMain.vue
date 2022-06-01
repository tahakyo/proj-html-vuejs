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
      <PopularFeatures :featuresCard="featuresCard" />
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
      featuresCard: [
        {
          title: "Customized Invoices",
          icon: "icon1.png",
        },
        {
          title: "Stock Management",
          icon: "icon2.png",
        },
        {
          title: "Receivable § Payables",
          icon: "icon3.png",
        },
        {
          title: "Manage Buying",
          icon: "icon4.png",
        },
        {
          title: "Powerful & Secure",
          icon: "icon5.png",
        },
        {
          title: "Fastest Return Filing",
          icon: "icon3.png",
        },
        {
          title: "Monthly Detailed",
          icon: "icon7.png",
        },
        {
          title: "Product Management",
          icon: "icon8.png",
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