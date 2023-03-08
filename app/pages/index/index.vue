<template>
	<view class="home">
			<scroll-view scroll-x class="navscroll">
				<view class="item">生肉</view>
				<view class="item">熟肉</view>
				<view class="item">新番</view>
				<view class="item">旧番</view>
				<view class="item">表番</view>
				<view class="item">里番</view>
			</scroll-view>
			
			<view class="content">
				<!-- 组件，自动引入的 -->
				<!-- <view class="row" v-for="item in 10">
					<newsbox></newsbox>
				</view> -->
				<div class="row" v-for="item in 10">
					<newsbox></newsbox>
				</div>
			</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			};
		}
	}
</script >

<style lang="scss">
.navscroll{
	width: 100%;
	height: 100rpx;
	background: #f7f8fa;
	white-space:nowrap;//不换行
	/deep/ ::-webkit-scrollbar{//去掉导航栏下的滑动条
		width: 4px !important;
		height: 1px !important;
		overflow: auto !important;
		 background: transparent !important;
		 -webkit-appearance: auto !important;
		 display: block;
	}
	.item{
		font-size: 40rpx;
		display: inline-block;
		line-height: 100rpx;
		padding: 0 30rpx;
		color: #333;
	}
}
.content{
		padding:30rpx;
		.row{
			border-bottom: 1px dotted #efefef;
			padding: 15rpx 0;
		}
	}
</style>