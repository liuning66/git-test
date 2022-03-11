<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<text class="title">{{title}}</text>
		</view>
		<button type="primary" size="mini" @click="handleBtnClick">点击跳转</button>


	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		beforeCreate() {
			console.log("index beforeCreate")
		},
		created() {
			console.log("index created")
		},
		beforeMount() {
			console.log("index beforeMount")
		},
		mounted() {
			console.log("index mounted")
		},
		beforeDestroy() {
			console.log("index beforeDestroy")
		},
		destroyed() {
			console.log("index destroyed")
		},


		onLoad() {
			console.log("index load")
		},
		onShow() {
			console.log("index show")
		},

		onReady() {
			console.log("index ready")
		},
		onHide() {
			console.log("index hide");
		},
		onUnload() {
			console.log("index unload")
		},
		methods: {
			handleBtnClick() {
				uni.navigateTo({
					url: "../test2/test2",
				})
			}
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
</style>
