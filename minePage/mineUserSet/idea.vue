<template>
	<view>
		<view class="title">
			标题
		</view>
		<view class="input-title">
			<input type="text" value="" placeholder="请输入意见标题" />
		</view>
		<view class="title">
			内容
		</view>
		<textarea class="content" placeholder="请输入意见内容" 
		placeholder-style="font-size:28rpx;font-family:PingFangSC-Regular,PingFang SC;font-weight:400;color:rgba(184,184,184,1);line-height:40rpx;" maxlength="-1"></textarea>
		<view class="button">提交</view>
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
.title{
	margin:30rpx 0 18rpx 30rpx;
	width:80rpx;
	height:56rpx;
	font-size:40rpx;
	font-family:PingFangSC-Semibold,PingFang SC;
	font-weight:600;
	color:rgba(55,55,55,1);
	line-height:56rpx;
}
.input-title{
	width:686rpx;
	height:94rpx;
	border-radius:8rpx;
	border:2rpx solid rgba(218,218,218,1);
	margin:0 30rpx 0rpx 30rpx;
	>input{
		margin-left:6rpx;
		margin-top: 27rpx;
		height:40rpx;
		font-size:14px;
		font-family:PingFangSC-Regular,PingFang SC;
		font-weight:400;
		line-height:40rpx;
	}
}
.content{
	background: #FFFFFF;
	margin-left: 30rpx;
	width:645rpx;
	height:356rpx;
	border-radius:8rpx;
	border:2rpx solid rgba(218,218,218,1);
	
}
//提交
.button{
	margin: 100rpx 108rpx 0 108rpx;
	width:534rpx;
	height:96rpx;
	background:rgba(164,211,255,1);
	border-radius:48rpx;
	border:4rpx solid rgba(235,246,255,1);
	text-align: center;
	justify-content: center;
	font-size:34rpx;
	font-family:PingFangSC-Semibold,PingFang SC;
	font-weight:600;
	color::rgba(255,255,255,1);
	line-height:96rpx;
}
</style>
