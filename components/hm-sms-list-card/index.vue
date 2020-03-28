<template>
  <div class="hm-sms-list-card">
    <div class="box">
      <image class="xueshengdangan" :src="options.xueshengdangan" />
      <image class="primary" :src="options.primary" />
      <div class="sub">
        <div class="outer">
          <div class="wrap">
            <text class="paybak">{{ options.paybak }}</text>
            <text class="company">{{ options.company }}</text>
          </div>
          <text class="txt">{{ options.txt }}</text>
        </div>
        <div class="block">
          <text class="desc">{{ options.desc }}</text>
        </div>
      </div>
      <image class="side" :src="options.side" />
    </div>
  </div>
</template>
<script>
export default {
  name: 'HmSmsListCard',
  props: {
    dataId: {
      type: String,
      default: 'hm-sms-list-card'
    },
    options: {
      type: Object,
      default: function() {
        return {
          xueshengdangan:
            '/static/hm-sms-list-card/images/img_25832_0_1.png',
          primary:
            '/static/hm-sms-list-card/images/img_25832_0_2.png',
          paybak: 'IM PAYBAK',
          company: '公司',
          txt: '3:46 PM',
          desc: '糟糕的星期三！通常用于演示',
          side:
            '/static/hm-sms-list-card/images/img_25832_0_0.png'
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
