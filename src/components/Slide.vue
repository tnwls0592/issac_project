<template>
<div id="wrap">
  <div class="inner">
  <swiper
      :spaceBetween="30"
      :centeredSlides="true"
      :autoplay="{
        delay: 2500,
        disableOnInteraction: false,
      }"
        :pagination="{
          clickable: true,
        }"
        :navigation="true"
        :modules="modules"
        class="mySwiper"
        >
    <swiper-slide>
      <img src="../assets/img/slide01.jpg" alt="">
      <div class="text01">
        <h1>특별한 달콤바삭함</h1><h2>치킨스페셜</h2><p>Chicken Special</p>
      </div>
    </swiper-slide>
    <swiper-slide>
      <img src="../assets/img/slide02.jpg" alt="">
      <div class="text02">
        <h1>일상을 부드럽게 채우는</h1><h2>스크램블 에그</h2>
      </div>
    </swiper-slide>
    <swiper-slide>
      <img src="../assets/img/slide03.jpg" alt="">
      <div class="text03">
        <h1>더 달콤하고 촉촉하게</h1><h2>프렌치 토스트</h2>
      </div>
    </swiper-slide>
    <swiper-slide>
      <img src="../assets/img/slide04.jpg" alt="">
      <div class="text04">
        <h1>새로운 Fried Menu</h1><h2>내일 또 생각나는<br>프라이드 토스트</h2>
      </div>
    </swiper-slide>
    <swiper-slide>
      <img src="../assets/img/slide05.jpg" alt="">
      <div class="text05">
        <h1>기억 속 오리지널 양념을 그대로</h1><h2>리얼 양념치킨</h2><p>신-메뉴</p>
      </div>
    </swiper-slide>
    <swiper-slide>
      <img src="../assets/img/slide06.jpg" alt="">
      <div class="text06">
        <h1>일상에 활기를 더하는 달콤한 한 입</h1><h2>소이크런치 치킨</h2>
      </div>
    </swiper-slide>
    ...
  </swiper>
  </div>
</div>
</template>
<script>
    // Import Swiper Vue.js components
  import { Swiper, SwiperSlide } from 'swiper/vue';

  // Import Swiper styles
  import 'swiper/css';

  import 'swiper/css/pagination';
  import 'swiper/css/navigation';

  // import required modules
  import { Autoplay, Pagination, Navigation } from 'swiper/modules';

  export default {
    components: {
      Swiper,
      SwiperSlide
    },
    setup() {
      return {
        modules: [Autoplay, Pagination, Navigation],
      };
    },
  };
</script>
<style lang="scss" scoped>
  @import '@/assets/scss/Slide.scss';
</style>