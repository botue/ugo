<template>
  <div>
    <!-- 搜索 -->
    <search></search>
    <!-- 分类 -->
    <div class="category">
      <!-- 顶级分类 -->
      <ul class="sup">
        <scroll-view scroll-y>
          <li class="active">大家电</li>
          <li>热门推荐</li>
          <li>海外购</li>
          <li>苏宁房产</li>
          <li>手机相机</li>
          <li>电脑办公</li>
          <li>厨卫电器</li>
          <li>食品酒水</li>
          <li>居家生活</li>
          <li>厨房电器</li>
        </scroll-view>
      </ul>
      <!-- 子级分类 -->
      <div class="sub">
        <scroll-view scroll-y>
          <!-- 封面图 -->
          <image src="/static/uploads/category.png" class="thumb"></image>
          <div class="children">
            <div class="title">电视</div>
            <!-- 品牌 -->
            <div class="brands">
              <navigator url="">
                <image src="/static/uploads/brand_1.jpg"></image>
                <span>曲面电视</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_2.jpg"></image>
                <span>海信</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_3.jpg"></image>
                <span>创维</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_4.jpg"></image>
                <span>夏普</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_5.jpg"></image>
                <span>TCL</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_6.jpg"></image>
                <span>PPTV</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_7.jpg"></image>
                <span>小米</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_8.jpg"></image>
                <span>长虹</span>
              </navigator>
            </div>
          </div>
          <div class="children">
            <div class="title">电视</div>
            <!-- 品牌 -->
            <div class="brands">
              <navigator url="">
                <image src="/static/uploads/brand_1.jpg"></image>
                <span>曲面电视</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_2.jpg"></image>
                <span>海信</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_3.jpg"></image>
                <span>创维</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_4.jpg"></image>
                <span>夏普</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_5.jpg"></image>
                <span>TCL</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_6.jpg"></image>
                <span>PPTV</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_7.jpg"></image>
                <span>小米</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_8.jpg"></image>
                <span>长虹</span>
              </navigator>
            </div>
          </div>
          <div class="children">
            <div class="title">电视</div>
            <!-- 品牌 -->
            <div class="brands">
              <navigator url="">
                <image src="/static/uploads/brand_1.jpg"></image>
                <span>曲面电视</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_2.jpg"></image>
                <span>海信</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_3.jpg"></image>
                <span>创维</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_4.jpg"></image>
                <span>夏普</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_5.jpg"></image>
                <span>TCL</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_6.jpg"></image>
                <span>PPTV</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_7.jpg"></image>
                <span>小米</span>
              </navigator>
              <navigator url="">
                <image src="/static/uploads/brand_8.jpg"></image>
                <span>长虹</span>
              </navigator>
            </div>
          </div>
        </scroll-view>
      </div>
    </div>
  </div>
</template>

<style scoped lang="less">

  scroll-view {
    height: 100%;
  }

  .category {
    display: flex;
    width: 100%;
    position: absolute;
    top: 100rpx;
    bottom: 0;

    .sup {
      width: 196rpx;
      background-color: #f4f4f4;

      li {
        height: 100rpx;
        text-align: center;
        line-height: 100rpx;
        font-size: 27rpx;
        color: #333;
        border-bottom: 1rpx solid #eee;

        &:last-child {
          border-bottom: none;
        }
        
        &.active {
          background-color: #FFF;
          color: #ea4451;
          position: relative;

          &::before {
            content: '';
            display: block;
            width: 8rpx;
            height: 60rpx;
            transform: translateY(-50%);
            background-color: #ea4451;

            position: absolute;
            left: 0;
            top: 50%;
          }
        }
      }
    }

    .sub {
      flex: 1;
      padding: 20rpx 18rpx;

      .thumb {
        width: 100%;
        height: 180rpx;
      }

      .children {
        text-align: center;
        color: #333;

        .title {
          display: inline-block;
          margin: 40rpx 0 20rpx;
          font-size: 30rpx;

          &::before {
            content: '/';
            margin-right: 20rpx;
            color: #666;
          }

          &::after {
            content: '/';
            margin-left: 20rpx;
            color: #666;
          }
        }
      }

      .brands {
        display: flex;
        flex-wrap: wrap;

        navigator {
          width: 33%;
          margin-bottom: 20rpx;
        }

        image {
          width: 120rpx;
          height: 120rpx;
        }

        span {
          display: block;
          font-size: 24rpx;
        }
      }
    }
  }
</style>

<script>

  import search from '@/components/search';

  export default {
    
    components: {
      search
    }
  }
</script>