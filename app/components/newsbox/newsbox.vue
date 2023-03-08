<template>
	<view class="newsbox">
		<view class="pic">
			<image src="../../static/images/0.jpg" mode="aspectFill"></image>
		</view>
		<view class="text">
			<view class="title">初音冲锋小号;初音冲锋小号;初音冲锋小号;初音冲锋小号;初音冲锋小号</view>
			<view class="info">
				<text>作者：Kieed</text>
				<text>998浏览</text>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		name:"newsbox",
		data() {
			return {
				
			};
		}
	}
</script>

<style lang="scss">
.newsbox{
	display: flex;//弹性布局
	.pic{
		width: 230rpx;
		height: 160rpx;
		image{
			width: 100%;
			height: 100%;
		}
	}
	.text{
		flex: 1;
		padding-left: 20rpx;
		display: flex;
		flex-direction:column;
		justify-content: space-between;
		.title{
			font-size: 38rpx;
			color: #333;
			//文本超出部分以...形式展示
			text-overflow: -o-ellipsis-lastline;
			//整体超出部分隐藏
			overflow: hidden;
			//文本超出部分以...形式展示，同第一行样式代码
			text-overflow: ellipsis;
			//display 块级元素展示
			display: -webkit-box;
			//设置文本行数为2行
			-webkit-line-clamp: 2;
			//设置文本行数为2行
			line-clamp: 2;
			//从上到下垂直排列子元素（设置伸缩盒子的子元素排列方式）
			-webkit-box-orient: vertical;
		}
		.info{
			font-size: 26rpx;
			color: #999; 
			text{
				padding-right: 30rpx;
			}
		}
	}
}
</style>