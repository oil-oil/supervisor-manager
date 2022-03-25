<template>
    <view class="cu-bar bg-white solid-bottom">
        <view class="action">
            <text class="cuIcon-titles text-blue"></text>
            {{ text }}
        </view>
        <view class="action">
            <slot></slot>
        </view>
    </view>
</template>

<script setup lang="ts">
import { defineProps } from 'vue';
const props = defineProps<{
    text: string
}>()
</script>

<style lang="scss" scoped>
</style>