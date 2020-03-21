<template>
	<view>
		<view class="mine-info">
			<span>修改头像</span>
			<view class="border"></view>
			<image class="img1" src="../../static/img/touxiang.png" mode=""></image>
			<image class="img2" src="../../static/img/mineIcon/jiantou.png" mode=""></image>
		</view>
		<view class="set-list">
			<view class="border"></view>
			<span>草稿箱</span>
			<image src="../../static/img/mineIcon/jiantou.png" mode="" @tap="goPage('drafts')"></image>
		</view>
		<view class="set-list">
			<view class="border"></view>
			<span>通知设置</span>
			<image src="../../static/img/mineIcon/jiantou.png" mode=""></image>
		</view>
		<view class="set-list">
			<view class="border"></view>
			<span>意见箱</span>
			<image src="../../static/img/mineIcon/jiantou.png" @tap="goPage('idea')" mode=""></image>
		</view>
		<view class="set-list">
			<view class="border"></view>
			<span>关于我们</span>
			<image src="../../static/img/mineIcon/jiantou.png" mode="" @tap="goPage('about')"></image>
		</view>
		
		<view class="button">退出</view>
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
			}
		}
	}
</script>

<style lang="scss" scoped>
.mine-info{
	width:750rpx;
	height:130rpx;
	position: relative;
	background:rgba(255,255,255,1);
	.border{
		position: absolute;
		top:0;
		left:30rpx;
		width:720rpx;
		height:126rpx;
		border-top: 2rpx solid rgba(241,241,241,1);
		border-bottom: 2rpx solid rgba(241,241,241,1);
	}
	>span{
		position: absolute;
		top:46rpx;
		left:30rpx;
		font-size:28rpx;
		height: 40rpx;
		font-family:PingFangSC-Regular,PingFang SC;
		font-weight:400;
		color:rgba(0,0,0,1);
	}
	.img1{
		position: absolute;
		top:26rpx;
		right:98rpx;
		width:80rpx;
		height:80rpx;
	}
	.img2{
		position: absolute;
		bottom:48rpx;
		right:44rpx;
		width:20rpx;
		height: 34rpx;
	}
}
// 草稿箱等模块
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
//退出按钮
.button{
	margin: 100rpx 108rpx 0 108rpx;
	width:534rpx;
	height:96rpx;
	background:rgba(255,255,255,1);
	border-radius:48rpx;
	border:4rpx solid rgba(235,246,255,1);
	text-align: center;
	justify-content: center;
	font-size:34rpx;
	font-family:PingFangSC-Semibold,PingFang SC;
	font-weight:600;
	color:rgba(44,149,248,1);
	line-height:96rpx;
}
</style>
