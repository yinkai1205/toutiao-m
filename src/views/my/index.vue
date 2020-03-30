<template>
  <div class="my-container">
    <div class="header">
      <img
        class="mobile-img"
        src="~@/assets/mobile.png"
        @click="$router.push('/login')"
      >
    </div>
    <!-- <div class="grid-nav"></div> -->
    <van-grid class="grid-nav">
      <van-grid-item
        class="grid-item"
        icon="shoucang"
      >
        <i slot="icon" class="toutiao toutiao-shoucang"></i>
        <span slot="text" class="text">收藏</span>
      </van-grid-item>
      <van-grid-item
        class="grid-item"
        icon="photo-o"
      >
        <span slot="text" class="text">历史</span>
        <i slot="icon" class="toutiao toutiao-lishi"></i>
      </van-grid-item>
      <van-grid-item
        class="grid-item"
      >
        <i slot="icon" class="toutiao toutiao-zuopin"></i>
        <span slot="text" class="text">作品</span>
      </van-grid-item>
    </van-grid>
    <van-cell title="消息通知" is-link url="" />
    <van-cell title="实名认证" is-link url="" />
    <van-cell title="用户反馈" is-link url="" />
    <van-cell title="小智同学" is-link url="" />
    <van-cell title="系统设置" is-link url="" />
  </div>
</template>

<script>
export default {
  name: 'MyIndex',
  components: {},
  props: {},
  data () {
    return {}
  },
  computed: {},
  watch: {},
  created () {},
  mounted () {},
  methods: {}
}
</script>

<style scoped lang="less">
.my-container {
  > .header {
    height: 361px;
    background: url("~@/assets/banner.png") no-repeat;
    background-size: cover;
    display: flex;
    justify-content: center;
    align-items: center;
    .mobile-img {
      width: 132px;
      height: 132px;
    }
  }

  .grid-nav {
    .grid-item {
      height: 141px;
      flex: 1;
      i.toutiao {
        font-size: 45px;
      }
      span.text {
        font-size: 28px;
        color: #333;
      }
    }
  }
}
</style>
