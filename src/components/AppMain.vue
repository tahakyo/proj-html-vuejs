<template>
  <section>
    <OnlineMarketingCard :marketingCard="marketingCard" />
    <TricksAndTips />
    <PopularFeatures :featuresCard="featuresCard" />
    <OurTestimonials :testimonialsCard="testimonialsCard" />
    <LatestPosts :latestPostsCard="latestPostsCard" />
    <AppContacts />
  </section>
</template>

<script>
import OnlineMarketingCard from "./OnlineMarketingCard.vue";
import TricksAndTips from "./TricksAndTips.vue";
import PopularFeatures from "./PopularFeatures.vue";
import OurTestimonials from "./OurTestimonials.vue";
import LatestPosts from "./latestPosts.vue";
import AppContacts from "./AppContacts.vue";
export default {
  name: "AppMain",
  components: {
    OnlineMarketingCard,
    TricksAndTips,
    PopularFeatures,
    OurTestimonials,
    LatestPosts,
    AppContacts,
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
      testimonialsCard: [
        {
          icon: "26.jpeg",
          name: "Julia Aann",
          profession: "Coo Sofbox",
          desc: "At vero eos et accusamus et iusto odio dignissimos At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur ducimus qui blanditiis praesentium vero eos et consectetur accus adip adi accus adip adip",
        },
        {
          icon: "27.jpeg",
          name: "Mac Znder",
          profession: "Manager sofbox",
          desc: "At vero eos et accusamus et iusto odio dignissimos At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur ducimus qui blanditiis praesentium vero eos et consectetur accus adip adi accus adip adip",
        },
      ],
      latestPostsCard: [
        {
          thumb: "19.jpg",
          date: "November 28, 2019",
          title: "Life Lack Meaning",
          text: "It is a long established fact that a reader will be distracted by the readable.",
        },
        {
          thumb: "18.jpg",
          date: "November 28, 2019",
          title: "Life Lack Meaning",
          text: "It is a long established fact that a reader will be distracted by the readable.",
        },
        {
          thumb: "17.jpg",
          date: "November 28, 2019",
          title: "Life Lack Meaning",
          text: "It is a long established fact that a reader will be distracted by the readable.",
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