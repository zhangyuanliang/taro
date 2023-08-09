<template>
  <view class="index">
    <text>我是首页！多次点击：</text>
    <text @tap="toPage" class="blue">ToPage</text>
  </view>
</template>

<script setup>
import { navigateTo } from '@tarojs/taro'
const toPage = () => {
  navigateTo({
    url: '/pages/sub/index',
  })
}
</script>

<style>
.blue {
  color: rgb(80, 80, 231);
}
</style>
