<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="banner">
    <Banner></Banner>
    <TrendingProducts></TrendingProducts>
  </div>
</template>

<script>
import Banner from "../components/homepage/HomepageBanner.vue";
import TrendingProducts from "../components/homepage/TrendingProducts.vue";

export default {
  components: { Banner, TrendingProducts },
  data() {
    return {};
  },
};
</script>

<style>
h2 {
  color: red;
}
</style>
