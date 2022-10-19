<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="min-h-screen">
    <app-tabs class="w-11/12 lg:w-10/12 mx-auto mb-16" :tabList="tabList">
      <template v-slot:tabPanel-1> 
        <FindOffline></FindOffline>  
      </template>
      <template v-slot:tabPanel-2> Online Store </template>
    </app-tabs>
  </div>
</template>

<script>
import AppTabs from "../components/location/Tabs.vue";
import FindOffline from "../components/location/FindOffline.vue";

export default {
  components: {
    AppTabs,
    FindOffline
  },

  data() {
    return {
      tabList: ["Find Nearby", "Find Online"],
    };
  },
};
</script>
