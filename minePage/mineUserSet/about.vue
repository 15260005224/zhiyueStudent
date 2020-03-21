<template>
	<view>
		<view class="logo">
		<image src="../../static/img/touxiang.png" mode=""></image>
		</view>
		<view class="appName">知阅学堂</view>
		<view class="version">版本 v1.0.0</view>
		<view class="set-list">
			<view class="border"></view>
			<span>用户协议</span>
			<image src="../../static/img/mineIcon/jiantou.png" mode="" @tap="goPage('')"></image>
		</view>
		<view class="set-list">
			<view class="border"></view>
			<span>服务条款</span>
			<image src="../../static/img/mineIcon/jiantou.png" mode=""></image>
		</view>
		<view class="set-list">
			<view class="border"></view>
			<span>隐私设置</span>
			<image src="../../static/img/mineIcon/jiantou.png" @tap="goPage('')" mode=""></image>
		</view>
		<view class="set-list">
			<view class="border"></view>
			<span>联系我们</span>
			<image src="../../static/img/mineIcon/jiantou.png" mode="" @tap="goPage('')"></image>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style lang="scss" scoped>
.logo{
	margin-top: 100rpx;
	margin-left:216rpx;
	>image{
		width:320rpx;
		height:320rpx;
	}
}
.appName{
	margin-top: 20rpx;
	margin-left:272rpx;
	width:208rpx;
	height:74rpx;
	font-size:52rpx;
	font-family:PingFangSC-Semibold,PingFang SC;
	font-weight:600;
	color:rgba(55,55,55,1);
	line-height:74rpx;
}
.version{
	margin:20rpx 0 60rpx 306rpx;
	width:140rpx;
	height:40rpx;
	font-size:28rpx;
	font-family:PingFangSC-Regular,PingFang SC;
	font-weight:400;
	color:rgba(184,184,184,1);
	line-height:40rpx;
}
.set-list{
	width:750rpx;
	height:100rpx;
	position: relative;
	background:rgba(255,255,255,1);
	.border{
		position: absolute;
		top:0;
		left:30rpx;
		width:720rpx;
		height:98rpx;
		// border-top: 2rpx solid rgba(241,241,241,1);
		border-bottom: 2rpx solid rgba(241,241,241,1);
	}
	>span{
		position: absolute;
		top:30rpx;
		left:30rpx;
		height:40rpx;
		font-size:28rpx;
		font-family:PingFangSC-Regular,PingFang SC;
		font-weight:400;
		color:rgba(0,0,0,1);
	}
	>image{
		position: absolute;
		bottom:34rpx;
		right:44rpx;
		width:20rpx;
		height: 34rpx;
	}
}
</style>
