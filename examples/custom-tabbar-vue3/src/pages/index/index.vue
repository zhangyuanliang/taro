<template>
  <view class="index">
    <text>我是首页！</text>
    <text @tap="toPage">ToPage</text>
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
