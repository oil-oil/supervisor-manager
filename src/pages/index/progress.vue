<template>
    <view style="width: 100%;">
        <van-collapse :value="progressActive" @change="progressChange">
            <van-collapse-item v-for="(item, index) in 10" :name="index">
                <view class="flex align-center" slot="title">
                    <view>
                        <view class="cu-tag light bg-green">
                            <text class="cuIcon-playfill text-lg margin-right-xs"></text>已启动
                        </view>
                        <!-- <view class="cu-tag light bg-red">
                <text class="cuIcon-stop text-lg margin-right-xs"></text>已停止
                        </view>-->
                    </view>
                    <view class="margin-left-sm">测试进程</view>
                </view>

                <view class="padding-sm margin-xs bg-white solid">
                    <view class="flex align-center">
                        <text class="text-gray">启动命令：</text>
                        <text class="cu-tag">yarn install</text>
                    </view>

                    <view class="margin-top-sm">
                        <text class="text-gray">启动用户：</text>
                        <text>赵四</text>
                    </view>

                    <view class="margin-top-sm">
                        <text class="text-gray">优先级：</text>
                        <text>999</text>
                    </view>

                    <view class="margin-top-sm flex align-center">
                        <text class="text-gray">进程 ID：</text>
                        <text>123456</text>
                    </view>

                    <view class="margin-top-sm">
                        <button class="cu-btn bg-blue block lg light" @click="handleProgress">操作</button>
                    </view>
                </view>
            </van-collapse-item>
        </van-collapse>
    </view>
</template>

<script setup lang="ts">
import { ref } from "vue";
const progressActive = ref([''])
const progressChange = (e: any) => {
    progressActive.value = e.detail
}

const handleProgress = () => {
    uni.showActionSheet({
        itemList: ["启动", "修改", "删除"]
    })
}
</script>

<style scoped>
</style>