<template>
	<view>
		<scroll-view scroll-x class="bg-white nav">
			<view class="flex text-center">
				<view
					class="cu-item flex-sub text-sm"
					:class="index == TabCur ? 'text-blue cur' : ''"
					v-for="(item, index) in topbarArr"
					:key="index"
					@tap="tabSelect(index)"
				>{{ item }}</view>
			</view>
		</scroll-view>

		<view class="cu-form-group">
			<input placeholder="请输入服务器地址" name="input" />
			<text class="cuIcon-global text-blue"></text>
		</view>
		<view class="cu-form-group">
			<input placeholder="请输入密码" name="input" />
			<text class="cuIcon-lock text-blue"></text>
		</view>
		<view class="padding flex">
			<button class="cu-btn radius lg bg-blue" style="width: 100%;" @tap="login">登陆</button>
		</view>
	</view>
</template>

<script setup lang="ts">
import { ref } from "vue";
const TabCur = ref(0);
const scrollLeft = ref(0)

const topbarArr = ['登陆', '部署']

const tabSelect = (index: number) => {
	TabCur.value = index
	scrollLeft.value = index * 60
}

const login = () => {
	uni.redirectTo({ url: "../index/index" })
}
</script>

<style></style>
