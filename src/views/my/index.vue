<template>
  <div class="my-container">
    <div class="header">
      <img
        class="mobile-img"
        src="~@/assets/mobile.png"
        @click="$router.push('/login')"
      >
    </div>
    <div class="grid-nav mb-9">
      <div class="grid-item">
        <i class="toutiao toutiao-shoucang"></i>
        <span class="text">收藏</span>
      </div>
      <div class="grid-item">
        <i class="toutiao toutiao-lishi"></i>
        <span class="text">历史</span>
      </div>
      <div class="grid-item">
        <i class="toutiao toutiao-zuopin"></i>
        <span class="text">作品</span>
      </div>
    </div>
    <van-cell title="消息通知" is-link url="" />
    <van-cell class="mb-9" title="实名认证" is-link url="" />
    <van-cell title="用户反馈" is-link url="" />
    <van-cell title="小智同学" is-link url="" />
    <van-cell class="mb-9" title="系统设置" is-link url="" />
    <van-cell style="text-align: center;" title="退出登录" />
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

  > .grid-nav {
    display: flex;
    > .grid-item {
      flex: 1;
      height: 141px;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      background-color: #fff;
      position: relative;
      i.toutiao {
        font-size: 45px;
      }
      .toutiao-shoucang {
        color: #eb5253;
      }
      .toutiao-lishi {
        color: #ff9d1d;
      }
      .toutiao-zuopin {
        color: #678eff;
      }
      span.text {
        font-size: 28px;
        color: #333;
      }
      &:not(:last-child):after {
        position: absolute;
        right: 0;
        content: "";
        width: 1px;
        height: 102px;
        background-color: #edeff3;
      }
    }
  }

  .mb-9 {
    margin-bottom: 9px;
  }
}
</style>
