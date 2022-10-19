<template>
	<view class="main">
	
	
	<view class="login">
		
		<view class="kuang shadow">
				<view class="hint">后台管理</view>
			<open-data class="avatar-open" type="userAvatarUrl"></open-data> 

				<view class="form-group">
					<view class="title">账号：</view>
					<input placeholder="管理员账号" maxlength="30"  placeholder-class="phc" model:value="{{username}}"></input>
				</view>
	
				<view class="form-group">
					<view class="title">密码：</view>
					<input placeholder="管理员密码" maxlength="30" type="password" placeholder-class="phc" model:value="{{password}}"></input>
				</view>
	
				<button class="btn" bindtap="bindGetPhoneNumber">点击登录</button>
			<view bindtap="url" data-url="../me/me" class="return">返回</view>
		</view>
	
	</view>
	
	<view class="bottom">
		 
	</view>
	
	</view>
</template>

<script>
	export default {
		data() {
			return {
				username:''
			};
		}
	}
</script>

<style lang="scss">
  .main {
  	width: 100%;
  	height: 100vh;
  	background-color: #0E9489;
  	display: flex;
  	flex-direction: column;
  	justify-content: flex-start;
  }
  
  .main .login {
  	margin-top: 150rpx;
  	display: flex;
  	flex-direction: column;
  	justify-content: flex-start;
  	align-items: center;
  	flex: 1;
  } 
  
  .main .login .kuang {
  	width: 600rpx;
  	background-color: #fff;
  	height: 750rpx;
  	margin-top: 0rpx;
  	border-radius: 20rpx;
  	display: flex;
  	flex-direction: column;
  	justify-content: space-between;
  	align-items: center;
  	padding: 50rpx 20rpx;
  }
  
  .main .login .kuang button {
  	width: 85%;
  	background-color: #0E9489;
  	color: #fff;
  	font-size:32rpx;
  }
  
  .main .login .kuang .hint {
  	width: 100%;
  	color: #aaa;
  	font-size:30rpx;
  	text-align: center;
  }
  
  .main .login .kuang .return {
  	width: 100%;
  	color: #0E9489;
  	font-size:30rpx;
  	text-align: center;
  	font-size:26rpx;
  }
  
  .main .avatar-open {
  	width: 180rpx;
  	height: 180rpx;
  	clip-path: circle(90rpx at center);
  }
  
  .main .bottom {
  	width: 100%;
  	align-self: flex-end;
  	font-size: 26rpx;
  	height: 70rpx;
  	text-align: center;
  	color: #fff;
  	display: flex;
  	flex-direction: column;
  }
  .form-group .title {
  	font-weight: normal;
  }
</style>
