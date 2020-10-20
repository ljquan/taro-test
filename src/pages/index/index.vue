<template>
  <view>view 标签</view>
  <div>div标签</div>
  <article>article标签</article>
  <text>text 标签，前面应该有div和article标签</text>
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
