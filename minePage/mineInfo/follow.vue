<template>
	<view>
		<view class="follow-box" v-for="(item,index) in 2">
			<image src="../../static/img/touxiang.png" mode=""></image>
			<view class="name">
				{{name}}
				<span>关注了你</span>
			</view>
			<view class="time">
				{{time}}
			</view>
			<view v-if="flag===1" class="danyi"><span>＋关注</span></view>
			<view v-if="flag===2" class="xianghu"><span>相互关注</span></view>
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				flag:1,
				name:'小章',
				time:'昨天 01:12'
			}
		},
		methods: {
	
		}
	}
</script>

<style lang="scss" scoped>
.follow-box{
	margin-top: 10rpx;
	width:750rpx;
	height:130rpx;
	background:rgba(246,248,250,1);
	position: relative;
	>image{
		position: absolute;
		top:26rpx;
		left:30rpx;
		width:40px;
		height:40px;
	}
	.name{
		position: absolute;
		top:30rpx;
		left:130rpx;
		// width:px;
		height:34rpx;
		font-size:24rpx;
		font-family:PingFangSC-Regular,PingFang SC;
		font-weight:400;
		color:rgba(55,55,55,1);
		line-height:34rpx;
		>span{
			margin-left: 10rpx;
		}
	}
	.time{
		position: absolute;
		top:68rpx;
		left:130rpx;
		width:112rpx;
		height:34rpx;
		font-size:24rpx;
		font-family:PingFangSC-Regular,PingFang SC;
		font-weight:400;
		color:rgba(184,184,184,1);
		line-height:34rpx;
	}
	.danyi{
		position: absolute;
		top:40rpx;
		right:60rpx;
		width:140rpx;
		height:50rpx;
		border-radius:26rpx;
		background:rgba(44,149,248,1);
		text-align: center;
		>span{
			font-size:24rpx;
			font-family:PingFangSC-Regular,PingFang SC;
			font-weight:400;
			color:rgba(255,255,255,1);
			line-height:34rpx;
		}
	
	}
	.xianghu{
		position: absolute;
		top:40rpx;
		right:60rpx;
		width:140rpx;
		height:50rpx;
		background:rgba(235,246,255,1);
		border-radius:26rpx;
		text-align: center;
		>span{
			font-size:24rpx;
			font-family:PingFangSC-Regular,PingFang SC;
			font-weight:400;
			color:rgba(164,211,255,1);
			line-height:34rpx;
		}

	}
}
</style>
