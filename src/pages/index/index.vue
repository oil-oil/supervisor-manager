<template>
  <view>
    <view class="radius">
      <Title text="守护进程管理">
        <view class="cu-btn bg-blue shadow-blur radius">添加</view>
      </Title>
      <Progress></Progress>
      <Title text="实时日志" />
      <Log></Log>
    </view>
  </view>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import Title from "../../components/title/index.vue"
import Progress from "./Progress.vue"
import Log from "./Log.vue"

</script>

<style>
</style>
