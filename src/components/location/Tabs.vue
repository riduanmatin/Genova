<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div
    :class="{
      'flex space-x-4': variant === 'horizontal',
    }"
  >
    <ul
      class="flex justify-center list-none bg-opacity-30 p-1.5 rounded-lg text-center overflow-auto whitespace-nowrap"
      :class="{
        'flex mb-5': variant === 'vertical',
      }"
    >
      <li
        v-for="(tab, index) in tabList"
        :key="index"
        class="w-1/4 px-6 py-1"
        :class="{
          'text-black font-bold underline underline-offset-8':
            index + 1 === activeTab,
          'text-black': index + 1 !== activeTab,
        }"
      >
        <!-- <label
          :for="`${_uid}${index}`"
          v-text="tab"
          class="cursor-pointer block"
        /> -->
        <label
          :for="`${index}`"
          v-text="tab"
          class="cursor-pointer block"
        />
        <!-- <input
          :id="`${_uid}${index}`"
          type="radio"
          :name="`${_uid}-tab`"
          :value="index + 1"
          v-model="activeTab"
          class="hidden"
        /> -->
        <input
          :id="`${index}`"
          type="radio"
          :name="`-tab`"
          :value="index + 1"
          v-model="activeTab"
          class="hidden"
        />
      </li>
    </ul>

    <template v-for="(tab, index) in tabList">
      <div :key="index" v-if="index + 1 === activeTab" class="flex-grow">
        <slot :name="`tabPanel-${index + 1}`" />
      </div>
    </template>
  </div>
</template>

<script>
export default {
  props: {
    tabList: {
      type: Array,
      required: true,
    },
    variant: {
      type: String,
      required: false,
      default: () => "vertical",
      validator: (value) => ["horizontal", "vertical"].includes(value),
    },
  },
  data() {
    return {
      activeTab: 1,
    };
  },
};
</script>

<style>
.flex {
  display: flex;
}
</style>
