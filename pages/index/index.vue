<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<text class="title">{{title}}1</text>
			<text>{{globalText}}</text>
		</view>
		<view>
			<van-button type="primary">按钮</van-button>
		</view>
		<view>
			<navigator url="/pages/about/index/index">跳转链接</navigator>
		</view>
		<view class="box"></view>
	</view>
</template>

<script>
	const app = getApp()
	export default {
		data() {
			return {
				title: 'Hello',
				globalText: app.globalData.globalText
			}
		},
		onLoad() {
			console.log(app.globalData)
		},
		onShow() {
			console.log("onShow")
		},
		onReady() {
			console.log("onReady")
		},
		methods: {

		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
	.box {
		width: 100rpx;
		height: 100rpx;
		background: red;
	}
</style>
