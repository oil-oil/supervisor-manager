<template>
    <view>
        <van-cell-group>
            <van-field v-model="form.name" placeholder="请输入用户名" />
        </van-cell-group>
    </view>
</template>

<script setup lang="ts">
import { reactive } from 'vue';

const form = reactive({
    name: "",
    user: "",
    path: "",
    command: "",
    procressNum: ""
})
</script>

<style scoped>
</style>