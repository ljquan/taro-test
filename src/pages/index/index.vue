<template>
  <view>View 标签</view>
  <div>Div标签</div>
  <text>Text 标签，前面应该有Div标签</text>
</template>

<script>
import { AtAccordion, AtList, AtListItem } from "taro-ui-vue3";
export default {
  name: "AccordionDemo",
  components: {
    AtAccordion,
    AtList,
    AtListItem,
  },
  data() {
    return {
      value1: false,
    };
  },
  methods: {
    onClick(val) {
      this.value1 = val;
    },
  },
};
</script>

<style lang="scss">
@import "taro-ui-vue3/dist/style/components/accordion.scss";
@import "taro-ui-vue3/dist/style/components/icon.scss";
</style>
