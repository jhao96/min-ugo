<template>
  <view class="content">
    <!-- 搜索 -->
    <view class="search">
      <view class="input-box">
        <input type="text" placeholder="搜索" />
      </view>
      <view class="content"></view>
    </view>
    <!-- 焦点图 -->
    <view class="slider"></view>
    <!-- 主导航 -->
    <view class="navs"></view>
    <!-- 楼层 -->
    <view class="floors"></view>
  </view>
</template>

<script>
export default {
  data() {
    return {
      title: "Hello",
      list: ["html", "css", "java"]
    };
  },
  onLoad() {
    console.log("当前页面加载了");
  },
  methods: {
    btn(res) {
      this.title = "你好";
      console.log(res);
    }
  }
};
</script>

<style lang="less">
.search {
  .input-box {
    padding: 20rpx 16rpx;
	background-color: #eb4450;
	input{
		background-color: #fff;
		border-radius: 10rpx;
		height: 60rpx;
		text-align: center;
	}
  }
}
</style>
