<template>
  <div class="wrapper">
    <!-- 个人资料 -->
    <div class="profile">
      <div class="meta">
        <img src="/static/uploads/monkey.png" class="avatar" alt="">
        <span>登录/注册</span>
      </div>
    </div>
    <!-- 统计 -->
    <div class="count">
      <div class="cell">
        0 <span>收藏的店铺</span>
      </div>
      <div class="cell">
        0 <span>收藏的商品</span>
      </div>
      <div class="cell">
        0 <span>关注的商品</span>
      </div>
      <div class="cell">
        0 <span>我的足迹</span>
      </div>
    </div>
    <!-- 我的订单 -->
    <div class="orders">
      <div class="title">我的订单</div>
      <div class="sorts">
        <span class="iconfont icon-daifukuan">待付款</span>
        <span class="iconfont icon-icon3">待收货</span>
        <span class="iconfont icon-icon5">退款/退货</span>
        <span class="iconfont icon-icon_order">全部订单</span>
      </div>
    </div>
    <!-- 地址管理 -->
    <div class="address">
      收货地址管理
    </div>
    <!-- 其它 -->
    <div class="extra">
      <div class="item">联系客服</div>
      <div class="item">意见反馈</div>
    </div>
  </div>
</template>

<style scoped lang="less">

  .wrapper {
    position: absolute;
    top: 0;
    bottom: 0;

    width: 100%;
    background-color: #f4f4f4;
  }

  .profile {
    height: 390rpx;
    background-color: #ea4451;
    display: flex;
    justify-content: center;
    align-items: center;

    .meta {

      .avatar {
        width: 140rpx;
        height: 140rpx;
        border-radius: 50%;
        border: 2rpx solid #fff;
      }

      span {
        display: block;
        text-align: center;
        margin-top: 20rpx;
        font-size: 24rpx;
        color: #fff;
      }
    }
  }

  .count {
    display: flex;
    margin: 0 20rpx;
    height: 100rpx;
    text-align: center;
    background-color: #fff;

    position: relative;
    top: -24rpx;

    .cell {
      flex: 1;
      padding-top: 16rpx;
      font-size: 24rpx;
      color: #666;
    }

    span {
      display: block;
    }
  }

  .orders {
    margin: 0 20rpx;
    padding: 20rpx 0;
    background-color: #fff;

    .title {
      padding-left: 20rpx;
      font-size: 30rpx;
      color: #333;
      padding-bottom: 20rpx;
      border-bottom: 1rpx solid #eee;
    }

    .sorts {
      padding-top: 30rpx;
      text-align: center;
      display: flex;
    }

    .iconfont {
      flex: 1;
      font-size: 27rpx;

      &::before {
        display: block;
        font-size: 48rpx;
        color: #ea4451;
      }
    }
  }

  .address {
    height: 88rpx;
    line-height: 88rpx;
    background-color: #fff;
    font-size: 30rpx;
    padding-left: 20rpx;
    margin: 20rpx;
    color: #333;
  }

  .extra {
    margin: 0 20rpx;
    background-color: #fff;

    .item {
      height: 88rpx;
      line-height: 88rpx;
      padding-left: 20rpx;
      border-bottom: 1rpx solid #eee;
      font-size: 30rpx;
      color: #333;
    }
  }
</style>

<script>
  export default {
    
  }
</script>