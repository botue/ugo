<template>
  <div :style="{height: pageHeight, overflow: 'hidden'}">
    <search @search="disableScroll"></search>
    <!-- 焦点图 -->
    <swiper class="banner" indicator-dots indicator-color="rgba(255, 255, 255, 0.6)" indicator-active-color="#fff">
      <swiper-item>
        <a href="">
          <img src="/static/uploads/banner1.png" />
        </a>
      </swiper-item>
      <swiper-item>
        <a href="">
          <img src="/static/uploads/banner2.png" />
        </a>
      </swiper-item>
      <swiper-item>
        <a href="">
          <img src="/static/uploads/banner3.png" />
        </a>
      </swiper-item>
    </swiper>
    <!-- 导航条 -->
    <div class="navs">
      <a href="">
        <img src="/static/uploads/icon_index_nav_1@2x.png" />
      </a>
      <a href="">
        <img src="/static/uploads/icon_index_nav_2@2x.png" />
      </a>
      <a href="">
        <img src="/static/uploads/icon_index_nav_3@2x.png" />
      </a>
      <a href="">
        <img src="/static/uploads/icon_index_nav_4@2x.png" />
      </a>
    </div>
    <!-- 楼层 -->
    <div class="floors">
      <div class="floor">
        <div class="title">
          <img src="/static/uploads/pic_floor01_title.png" />
        </div>
        <div class="items">
          <a href="">
            <img src="/static/uploads/pic_floor01_1@2x.png" />
          </a>
          <a href="">
            <img src="/static/uploads/pic_floor01_2@2x.png" />
          </a>
          <a href="">
            <img src="/static/uploads/pic_floor01_3@2x.png" />
          </a>
          <a href="">
            <img src="/static/uploads/pic_floor01_4@2x.png" />
          </a>
          <a href="">
            <img src="/static/uploads/pic_floor01_5@2x.png" />
          </a>
        </div>
      </div>
      <div class="floor">
        <div class="title">
          <img src="/static/uploads/pic_floor02_title.png"/>
        </div>
        <div class="items">
          <a href="">
            <img src="/static/uploads/pic_floor02_1@2x.png" />
          </a>
          <a href="">
            <img src="/static/uploads/pic_floor02_2@2x.png" />
          </a>
          <a href="">
            <img src="/static/uploads/pic_floor02_3@2x.png" />
          </a>
          <a href="">
            <img src="/static/uploads/pic_floor02_4@2x.png" />
          </a>
          <a href="">
            <img src="/static/uploads/pic_floor02_5@2x.png" />
          </a>
        </div>
      </div>
      <div class="floor">
        <div class="title">
          <img src="/static/uploads/pic_floor03_title.png" />
        </div>
        <div class="items">
          <a href="">
            <img src="/static/uploads/pic_floor03_1@2x.png" />
          </a>
          <a href="">
            <img src="/static/uploads/pic_floor03_2@2x.png" />
          </a>
          <a href="">
            <img src="/static/uploads/pic_floor03_3@2x.png" />
          </a>
          <a href="">
            <img src="/static/uploads/pic_floor03_4@2x.png" />
          </a>
          <a href="">
            <img src="/static/uploads/pic_floor03_5@2x.png" />
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

  import search from '@/components/search'

  export default {

    data () {
      return {
        pageHeight: 'auto'
      }
    },

    components: {
      search
    },
    
    methods: {
      disableScroll (ev) {
        this.pageHeight = ev.pageHeight + 'px';
      }
    }
  }
</script>

<style scoped lang="less">

  .banner {
    width: 100%;
    height: 340rpx;

    img {
      width: 100%;
      height: 340rpx;
    }
  }

  .navs {
    display: flex;
    justify-content: space-between;
    padding: 30rpx 44rpx;

    img {
      width: 128rpx;
      height: 140rpx;
    }
  }

  .floors {

    .title {
      width: 750rpx;
      height: 60rpx;
      padding-top: 20rpx;
      background-color: #f4f4f4;
    }

    .items {
      padding: 20rpx 16rpx;
      overflow: hidden;

      a {
        width: 232rpx;
        height: 188rpx;
        margin-right: 10rpx;
        margin-bottom: 10rpx;
        float: left;
      }

      a:nth-child(2n+1) {
        margin-right: 0;
      }

      a:first-child {
        height: 386rpx;
        margin-right: 10rpx;
      }
    }
  }

</style>
