<template>
    <view class="padding-sm margin-sm bg-white shadow">
        <view class="flex justify-between align-center margin-top-sm">
            <view class="text-bold text-black">进程名称</view>
            <view>
                <view class="cu-tag light bg-green">
                    <text class="cuIcon-playfill text-lg margin-right-xs"></text>已启动
                </view>
                <view class="cu-tag light bg-red">
                    <text class="cuIcon-stop text-lg margin-right-xs"></text>已停止
                </view>
            </view>
        </view>

        <view class="margin-top-sm flex align-center">
            <text>启动命令：</text>
            <text class="cu-tag">yarn install</text>
        </view>

        <view class="margin-top-sm">
            <text>启动用户：</text>
            <text>赵四</text>
        </view>
    </view>
</template>

<script setup lang="ts">

</script>

<style scoped>
</style>