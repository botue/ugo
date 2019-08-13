
<template>
  <div>
    <!-- 筛选 -->
    <div class="filter">
      <span class="active">综合</span>
      <span>销量</span>
      <span>价格</span>
    </div>
    <!-- 商品列表 -->
    <scroll-view class="goods" scroll-y>
      <div class="item">
        <!-- 商品图片 -->
        <image class="pic" src="/static/uploads/goods_1.jpg"></image>
        <!-- 商品信息 -->
        <div class="meta">
          <p class="name">【海外购自营】黎珐(ReFa) MTG日本 CARAT铂金微电流瘦脸瘦身提拉紧致V脸美容仪 【保税仓发货】</p>
          <p class="price"><span>￥</span>1399<span>.00</span></p>
        </div>
      </div>
      <div class="item">
        <!-- 商品图片 -->
        <image class="pic" src="/static/uploads/goods_2.jpg"></image>
        <!-- 商品信息 -->
        <div class="meta">
          <p class="name">卡奇莱德汽车车载空气净化器负离子除甲醛PM2.5除烟异味车用氧吧双涡轮出风（红色）</p>
          <p class="price"><span>￥</span>168<span>.00</span></p>
        </div>
      </div>
      <div class="item">
        <!-- 商品图片 -->
        <image class="pic" src="/static/uploads/goods_3.jpg"></image>
        <!-- 商品信息 -->
        <div class="meta">
          <p class="name">沿途（yantu）车载充电器车充一拖二usb转接口手机智能头多功能汽车点烟器</p>
          <p class="price"><span>￥</span>168<span>.00</span></p>
        </div>
      </div>
      <div class="item">
        <!-- 商品图片 -->
        <image class="pic" src="/static/uploads/goods_4.jpg"></image>
        <!-- 商品信息 -->
        <div class="meta">
          <p class="name">车载冰箱7.5L 冷暖两用汽车冰箱半导体12V迷你电冰箱升级款</p>
          <p class="price"><span>￥</span>168<span>.00</span></p>
        </div>
      </div>
      <div class="item">
        <!-- 商品图片 -->
        <image class="pic" src="/static/uploads/goods_5.jpg"></image>
        <!-- 商品信息 -->
        <div class="meta">
          <p class="name">神行者电子狗 神行者L70电子狗测速 测速雷达 流动测速 多种警示路段提醒</p>
          <p class="price"><span>￥</span>168<span>.00</span></p>
        </div>
      </div>
    </scroll-view>
  </div>
</template>

<style scoped lang="less">

  .filter {
    display: flex;
    height: 96rpx;
    line-height: 96rpx;
    border-bottom: 1rpx solid #ddd;

    span {
      flex: 1;
      text-align: center;
      font-size: 30rpx;
      color: #333;

      &.active {
        color: #ea4451;
      }
    }
  }
  
  .goods {
    position: absolute;
    width: 100%;
    top: 97rpx;
    bottom: 0;
  }

  .item {
    display: flex;
    padding: 30rpx 20rpx 30rpx 0;
    margin-left: 20rpx;
    border-bottom: 1rpx solid #eee;

    &:last-child {
      border-bottom: none;
    }

    .pic {
      width: 200rpx;
      height: 200rpx;
      margin-right: 30rpx;
    }

    .meta {
      flex: 1;
      font-size: 27rpx;
      color: #333;
      position: relative;
    }

    .name {
      width: 100%;
      overflow: hidden;
      text-overflow: ellipsis;
      display: -webkit-box;
      -webkit-line-clamp: 2;
      -webkit-box-orient: vertical;
    }

    .price {
      position: absolute;
      bottom: 0;

      color: #ea4451;
      font-size: 33rpx;

      span {
        font-size: 22rpx;
      }
    }
  }

</style>

<script>
  export default {

  }
</script>