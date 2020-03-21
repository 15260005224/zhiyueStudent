<template>
	<view>
		<view class="trends-box" v-for="(item,index) in 3">
			<image src="../../static/img/touxiang.png" mode=""></image>
			<view class="name">
				{{name}}
				<span>同学完成</span>
				<span style="color:#4E8ECF;">《{{bookname}}》</span>
				<span>老师布置的</span>{{pubulicType}}
			</view>
			<view class="time">
				{{time}}
			</view>
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				pubulicType:'考试',
				bookname:'十万个为什么',
				flag:1,
				name:'小章',
				time:'2020年2月20日'
			}
		},
		methods: {
	
		}
	}
</script>

<style lang="scss" scoped>
.trends-box{
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
		// width:112rpx;
		height:34rpx;
		font-size:24rpx;
		font-family:PingFangSC-Regular,PingFang SC;
		font-weight:400;
		color:rgba(184,184,184,1);
		line-height:34rpx;
	}
}
</style>
