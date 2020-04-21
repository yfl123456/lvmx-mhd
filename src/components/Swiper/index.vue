<template>
  <!-- banner -->
  <div class="swiper-container">
    <div class="swiper-wrapper">
      <!-- <div class="swiper-slide">Slide 1</div>
      <div class="swiper-slide">Slide 2</div>
      <div class="swiper-slide">Slide 3</div> -->
      <slot />
    </div>
    <!-- 如果需要分页器 -->
    <div class="swiper-pagination"></div>
  </div>
  <!-- banner end -->
</template>

<script>
import Swiper from 'swiper'
import 'swiper/css/swiper.css'

export default {
  name: 'Swiper',
  /* eslint-disable */
  mounted() {
    new Swiper('.swiper-container', {
      loop: true, // 循环模式选项
      // 分页器
      pagination: {
        el: '.swiper-pagination'
      },
      autoplay: true // 自动切换
    })
  }
  /* eslint-enable */
}
</script>

<style lang="scss" scoped>
.swiper-container {
  width: 100%;
  height: 200px;
  background: red;
}
</style>
