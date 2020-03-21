<template>
	<view>
		<view class="set-list" v-for="(item,index) in 6">
			<view class="border"></view>
			<span>{{title}}</span>
			<view class="time">	{{time}}</view>
			<image src="../../static/img/mineIcon/jiantou.png" mode="" @tap="goPage('')"></image>
		</view>
	
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title:'我好像',
				time:'2020年2月20日 12:00'
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
		top:14rpx;
		left:30rpx;
		height:34rpx;
		font-size:24rpx;
		font-family:PingFangSC-Regular,PingFang SC;
		font-weight:400;
		color:rgba(55,55,55,1);
		line-height:34rpx;
	}
	.time{
		position: absolute;
		top:52rpx;
		left:30rpx;
		height:34rpx;
		font-size:24rpx;
		font-family:PingFangSC-Regular,PingFang SC;
		font-weight:400;
		color:rgba(218,218,218,1);
		line-height:34rpx;
	}
	>image{
		position: absolute;
		bottom:34rpx;
		right:46rpx;
		width:20rpx;
		height: 34rpx;
	}
}
.set-list:first-child{
		border-top: 2rpx solid rgba(241,241,241,1);
}
</style>
