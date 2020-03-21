<template>
	<view>
	<view class="content-box"  v-for="(item,index) in 3">
		<image src="../../static/img/touxiang.png" mode=""></image>
		<view class="name">
			<span>{{name}}</span>
			评论了你的{{typeName}}
		</view>
		<view class="time">
			{{time}}
		</view>
		<view class="title">
			{{title}}
		</view>
		<view class="content">
			{{content}}
		</view>
	</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				name:'小李',
				typeName:'作文',
				time:'2019年12月31日',
				title:'好书好看',
				content:'真的是牛批！真的是牛批！真的是牛批！真的是牛批！真的是牛批！真的是牛批！真的是牛批！真的是牛批！'
			}
		},
		methods: {
			
		}
	}
</script>

<style lang="scss" scoped>
.content-box{
	margin-top: 10rpx;
	width:750rpx;
	height:322rpx;
	background:rgba(246,248,250,1);	
	position: relative;
	>image{
		position: absolute;
		top:30rpx;
		left: 30rpx;
		width:80rpx;
		height:80rpx;
	}
	.name{
		position: absolute;
		top:34rpx;
		left: 130rpx;
		width:232rpx;
		height:34rpx;
		font-size:24rpx;
		font-family:PingFangSC-Regular,PingFang SC;
		font-weight:400;
		color:rgba(55,55,55,1);
		line-height:34rpx;
		>span{
			margin-right:8rpx
		}
	}
	.time{
		position: absolute;
		top:72rpx;
		left: 130rpx;
		width:174rpx;
		height:34rpx;
		font-size:24rpx;
		font-family:PingFangSC-Regular,PingFang SC;
		font-weight:400;
		color:rgba(184,184,184,1);
		line-height:34rpx;
	}
	.title{
		position: absolute;
		top:130rpx;
		left: 130rpx;
		width:140rpx;
		height:40rpx;
		font-size:28rpx;
		font-family:PingFangSC-Semibold,PingFang SC;
		font-weight:600;
		color:rgba(55,55,55,1);
		line-height:40rpx;
	}
	.content{
		position: absolute;
		top:180rpx;
		left: 110rpx;
		width: 590rpx;
		height:102rpx;
		font-size:24rpx;
		font-family:PingFangSC-Regular,PingFang SC;
		font-weight:400;
		color:rgba(55,55,55,1);
		background:rgba(246,248,250,1);	
		line-height:34rpx;
	}
	
}

</style>
