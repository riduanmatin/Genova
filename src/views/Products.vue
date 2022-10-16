<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <AppBanner />
  <Products></Products>
</template>

<script>
import Products from "../components/products/Products.vue";
import AppBanner from "../components/AppBanner.vue";

export default {
  // eslint-disable-next-line vue/no-unused-components
  components: { Products, AppBanner },
  data() {
    return {};
  },
};
</script>
