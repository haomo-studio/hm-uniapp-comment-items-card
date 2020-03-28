<template>
  <div class="hm-comment-items-card">
    <div class="primary">
      <div class="shopCreditWrap">
        <image class="shopCreditLv1" :src="options.shopCreditLv1" />
      </div>
      <text class="daysAgo">{{ options.daysAgo }}</text>
      <text class="info">{{ options.info }}</text>
    </div>
  </div>
</template>
<script>
export default {
  name: 'HmCommentItemsCard',
  props: {
    dataId: {
      type: String,
      default: 'hm-comment-items-card'
    },
    options: {
      type: Object,
      default: function() {
        return {
          shopCreditLv1:
            './images/img_25837_0_0.png',
          daysAgo: '3 days ago',
          info: '老王回复了您'
        };
      }
    }
  },
  data() {
    return {};
  },
  methods: {}
};
</script>
<style>
@import './index.response.css';
</style>
