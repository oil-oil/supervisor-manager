<template>
  <view>
    <view class="radius">
      <Title text="守护进程管理" />
      <Progress></Progress>
      <Title text="实时日志" />
      <Log></Log>
    </view>
  </view>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import Title from "../../components/title/index.vue"
import Progress from "./progress.vue"
import Log from "./log.vue"

</script>

<style>
</style>
