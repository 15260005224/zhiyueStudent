<template>
	<view >
	<view class="info-operation">
		<view class="operation" @tap="goPage('support')">
			<image src="../../static/img/mineIcon/dianzan.png" mode=""></image>
			 <view>点赞</view>
		</view>
		<view class="operation" @tap="goPage('follow')">
			<image src="../../static/img/mineIcon/guanzhu.png" mode=""></image>
			 <view>关注</view>
		</view>
		<view class="operation" @tap="goPage('comment')">
			<image src="../../static/img/mineIcon/pinglun.png" mode=""></image>
			 <view>评论与回复</view>
		</view>
	</view>
	<!-- 提醒模块 -->
	<view class="remind" @tap="goPage('trends')">
		<image src="../../static/img/mineIcon/dongtai.png" mode=""></image>
		 <view class="title">同学动态</view>
		 <view class="count-box">
		 	<view class="count">
		 		99
		 	</view>
		 </view>
	</view>
	<view class="remind" @tap="goPage('task')">
		<image src="../../static/img/mineIcon/renwu.png" mode=""></image>
		 <view class="title">任务提醒</view>
		<view class="count-box">
			<view class="count">
				99
			</view>
		</view>
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
			goPage(path){
				uni.navigateTo({
					url:'./'+path
				})
			},
		
		}
	}
</script>

<style lang="scss" scoped>
.info-operation{
	width:690rpx;
	height:170rpx;
	background:rgba(255,255,255,1);
	box-shadow:0px 4rpx 20rpx 0px rgba(188,216,238,0.5);
	border-radius:26rpx;
	margin:30rpx 30rpx 0 30rpx;
	display: flex;
	align-items: center;//子元素垂直居中
	justify-content: center;//子元素水平居中
	.operation{
		flex:1;
		 text-align: center;
		>image{
			vertical-align:middle;
			width:52rpx;
			height:56rpx;
	
		}
		>view{
			margin-top: 4rpx;
			height:40rpx;
			font-size:28rpx;
			font-family:PingFangSC-Regular,PingFang SC;
			font-weight:400;
			color:rgba(55,55,55,1);
			line-height:40rpx;
		}
	}
}
	// 提醒模块
.remind{
	width:690rpx;
	height:98rpx;
	background:rgba(255,255,255,1);
	box-shadow:0px 4rpx 20rpx 0px rgba(188,216,238,0.5);
	border-radius:26rpx;
	margin: 30rpx 30rpx 0 30rpx;
	align-items: center;//子元素垂直居中
	justify-content: center;
	>image{
		vertical-align: middle;
		width:52rpx;
		height:56rpx;
		padding: 20rpx;
		}
	.title{
		display: inline-block;
		// width:112rpx;
		height:40rpx;
		font-size:28rpx;
		font-family:PingFangSC-Regular,PingFang SC;
		font-weight:400;
		color:rgba(55,55,55,1);
		line-height:98rpx;
		}
	.count-box{
		display: inline-block;
		float: right;
		width:42rpx;
		height:42rpx;
		line-height: 42rpx;
		margin: 24rpx;
		background:rgba(255,63,63,1);
		border-radius: 42rpx;
		.count{
			margin: 8rpx;
			width:24rpx;
			height:28rpx;
			font-size:20rpx;
			font-family:PingFangSC-Regular,PingFang SC;
			font-weight:400;
			color:rgba(255,255,255,1);
			line-height:28rpx;
			}
		}	
		.count-box::after{
			clear: both;
			content: '';
		}
}
	
</style>
