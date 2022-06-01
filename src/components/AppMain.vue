<template>
  <div>
    <section>
      <OnlineMarketingCard :marketingCard="marketingCard" />
    </section>
    <section>
      <TricksAndTips />
    </section>

    <section>
      <PopularFeatures :featuresCard="featuresCard" />
    </section>
    <section>
      <OurTestimonials />
    </section>
  </div>
</template>

<script>
import OnlineMarketingCard from "./OnlineMarketingCard.vue";
import TricksAndTips from "./TricksAndTips.vue";
import PopularFeatures from "./PopularFeatures.vue";
import OurTestimonials from "./OurTestimonials.vue";
export default {
  name: "AppMain",
  components: {
    OnlineMarketingCard,
    TricksAndTips,
    PopularFeatures,
    OurTestimonials,
  },
  data: function () {
    return {
      marketingCard: [
        {
          logo: "24.png",
          title: "Online Marketing",
          text: "It's a long established fact that a reader will be distracted",
        },
        {
          logo: "24.png",
          title: "Online Marketing",
          text: "It's a long established fact that a reader will be distracted",
        },
        {
          logo: "24.png",
          title: "Online Marketing",
          text: "It's a long established fact that a reader will be distracted",
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