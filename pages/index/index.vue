<template>
	<view class="container">
    <view>手机号：{{fromData.phone}}</view>
    <view>密码：{{fromData.code}}</view>
	</view>
</template>

<script>
	export default {
	  setup(props,context){
		let fromData = {
			phone:'18218877158',
			code:'20020'
		}
		return { fromData }
	  }
	}
</script>

<style>
	.container {
		padding: 20px;
		font-size: 14px;
		line-height: 24px;
	}
</style>
