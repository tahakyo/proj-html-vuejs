<template>
  <div class="container">
    <div class="online_marketing">
      <OnlineMarketingCard />
      <OnlineMarketingCard />
      <OnlineMarketingCard />
    </div>
  </div>
</template>

<script>
import OnlineMarketingCard from './OnlineMarketingCard.vue';
export default {
    name: "AppMain",
    components: { OnlineMarketingCard }
};
</script>

<style lang="scss" scoped>
.online_marketing {
  margin-top: 7rem;
  display: flex;
  
}
</style>