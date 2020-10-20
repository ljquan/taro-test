<template>
  <AtAccordion @click="onClick" title="hello" :open="value1">
    <AtList :hasBorder="false">
      <AtListItem
        title="标题文字"
        thumb="https://img12.360buyimg.com/jdphoto/s72x72_jfs/t6160/14/2008729947/2754/7d512a86/595c3aeeNa89ddf71.png"
      />
      <AtListItem
        title="标题文字"
        note="描述信息"
        thumb="http://img12.360buyimg.com/jdphoto/s72x72_jfs/t10660/330/203667368/1672/801735d7/59c85643N31e68303.png"
      />
    </AtList>
  </AtAccordion>
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
@use "taro-ui-vue3/dist/style/components/accordion.scss";
@use "taro-ui-vue3/dist/style/components/icon.scss";
</style>
