<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
import PageLoader from "./components/PageLoader.vue";

export default {
  components: {
    AppHeader,
    AppFooter,
    PageLoader,
  },
  data: () => {
    return {};
  },
};
</script>

<template>
  <PageLoader />
  <div class="flex flex-col h-screen justify-between">
    <AppHeader class="top-0" />
    <Router-view class="mb-auto" />
    <AppFooter class="bottom-0" />
  </div>
</template>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}

.container-shadow {
  box-shadow: rgba(67, 71, 85, 0.27) 0px 0px 0.25em,
    rgba(90, 125, 188, 0.05) 0px 0.25em 1em;
}
</style>
