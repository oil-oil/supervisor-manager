<template>
  <view>
    <view class="radius">
      <Title text="守护进程管理" />
      <ProgressItem></ProgressItem>
    </view>
  </view>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import Title from "../../components/title/index.vue"
import ProgressItem from "./progress-item/index.vue"
</script>

<style>
</style>
