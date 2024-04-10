<template>
  <view class="index">
    <text>{{ msg }}</text>
    <Button @tap="handleClick">点我</Button>
  </view>
</template>

<script setup>
import { ref } from "vue";
import { Button } from "@tarojs/components";

import "./index.scss";
const msg = ref("Hello world");
const handleClick = () => {
  console.log("===> 你好");
  msg.value = "牛逼";
};
</script>
