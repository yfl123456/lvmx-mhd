<template>
  <div class="page-home">
    <!-- 头部 -->
    <header class="index-header">
      <a href="">
        <div class="header-user">
          <div class="user-btn"></div>
        </div>
      </a>
      <div class="header-logo"></div>
      <a href="">
        <div class="header-search"></div>
      </a>
    </header>
    <!-- 头部 end -->

    <!-- banner -->
    <Swiper />
    <!-- banner end -->
  </div>
</template>

<script>
import Swiper from '@/components/Swiper'

export default {
  name: 'Home',
  components: {
    Swiper
  }
}
</script>

<style lang="scss" scoped>
.page-home {
  display: flex;
  flex-direction: column;
  height: 100%;
}
.index-header {
  padding: 0 20px;
  box-sizing: border-box;
  display: flex;
  height: 44px;
  justify-content: space-between;
  align-items: center;
  .user-btn {
    width: 25px;
    height: 25px;
    background: url('../../assets/icon/user-btn.png') no-repeat center center;
    background-size: 100%;
  }
  .header-logo {
    width: 92px;
    height: 28px;
    background: url('../../assets/icon/logo.png') no-repeat center center;
    background-size: 100%;
  }
  .header-search {
    height: 25px;
    width: 25px;
    background: url('../../assets/icon/scoat.png') no-repeat center center;
    background-size: 100%;
  }
}
</style>
