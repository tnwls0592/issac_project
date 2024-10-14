<template>
  <div id="wrap" data-aos="fade-up" data-aos-duration="1500">
    <div class="inner">
      <p><img src="../assets/img/icon.png" alt=""></p>
      <h1>Isaac Toast Menu</h1>
      <ul class="list">
        <li><a href="#" v-for="(list,index) in lists" :key="index" @click="currentList = index" :class="{'active' : currentList === index}">{{list.name}}</a></li>
      </ul>
      <div class="slide" v-if="currentList === 0">
      <ul class="listToast">
        <li><a href="#">
          <img src="../assets/img/SlideToast/2306210026_M1.png" alt="">
          <div class="name">
            <h1>허니갈릭 햄치즈</h1>
            <p>Honey Garlic Ham Cheese</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideToast/2306210032_M1.png" alt="">
          <div class="name">
            <h1>콘치즈 토스트</h1>
            <p>Corn Cheese</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideToast/2408090003_M1.png" alt="">
          <div class="name">
            <h1>소이 크런치 치킨</h1>
            <p>Soy Crunch Chicken</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideToast/2406110001_M1.png" alt="">
          <div class="name">
            <h1>프렌치 스크램블</h1>
            <p>French Scrambled</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideToast/2404220003_M1.png" alt="">
          <div class="name">
            <h1>프렌치 햄치즈</h1>
            <p>French Ham Cheese</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideToast/2402160007_M1.png" alt="">
          <div class="name">
            <h1>스크렘블 더블모짜</h1>
            <p>Scrambled Double Mozzarella</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideToast/2402160004_M1.png" alt="">
          <div class="name">
            <h1>스크렘블 베이컨</h1>
            <p>Scrambled Bacon</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideToast/2406110001_M1.png" alt="">
          <div class="name">
            <h1>스크렘블 햄치즈</h1>
            <p>Scrambled Ham Cheese</p>
          </div>
        </a></li>
      </ul>
      <ul class="listToast02">
        <li><a href="#">
          <img src="../assets/img/SlideToast/2312080001_M1.png" alt="">
          <div class="name">
            <h1>리얼 양념치킨</h1>
            <p>Real Seasoned Spicy Chicken</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideToast/2306260002_M1.png" alt="">
          <div class="name">
            <h1>치킨 스페셜</h1>
            <p>Chicken Special</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideToast/2306260004_M1.png" alt="">
          <div class="name">
            <h1>핫베이컨 치킨</h1>
            <p>Hot Bacon Chicken</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideToast/2404220003_M1.png" alt="">
          <div class="name">
            <h1>햄치즈 토스트</h1>
            <p>Ham Cheese</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideToast/2306210009_M1.png" alt="">
          <div class="name">
            <h1>햄 스페셜 토스트</h1>
            <p>Ham Special</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideToast/2306210011_M1.png" alt="">
          <div class="name">
            <h1>베이컨 베스트</h1>
            <p>Bacon Best</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideToast/2306210028_M1.png" alt="">
          <div class="name">
            <h1>그릴드 불고기</h1>
            <p>Grilled Bulgogi</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideToast/2306210030_M1.png" alt="">
          <div class="name">
            <h1>그릴드 불갈비</h1>
            <p>Grilled Bulgalbi</p>
          </div>
        </a></li>
      </ul>
      </div>
      <div class="slide02" v-if="currentList === 1">
      <ul class="listToastSet">
        <li><a href="#">
          <img src="../assets/img/SlideSet/2306260009_M1.png" alt="">
          <div class="name">
            <h1>허니갈릭 햄치즈 세트</h1>
            <p>Honey Garlic Ham Cheese Set</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideSet/2306260015_M1.png" alt="">
          <div class="name">
            <h1>콘치즈 토스트 세트 Set</h1>
            <p>Corn Cheese</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideSet/2408090004_M1.png" alt="">
          <div class="name">
            <h1>소이 크런치 치킨 세트</h1>
            <p>Soy Crunch Chicken Set</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideSet/2404220006_M1.png" alt="">
          <div class="name">
            <h1>프렌치 스크램블 세트</h1>
            <p>French Scrambled Set</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideSet/2404220005_M1.png" alt="">
          <div class="name">
            <h1>프렌치 햄치즈 세트</h1>
            <p>French Ham Cheese Set</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideSet/2402160009_M1.png" alt="">
          <div class="name">
            <h1>스크렘블 더블모짜 세트</h1>
            <p>Scrambled Double Mozzarella Set</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideSet/2402160006_M1.png" alt="">
          <div class="name">
            <h1>스크렘블 베이컨 세트</h1>
            <p>Scrambled Bacon Set</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideSet/2402160003_M1.png" alt="">
          <div class="name">
            <h1>스크렘블 햄치즈</h1>
            <p>Scrambled Ham Cheese Set</p>
          </div>
        </a></li>
      </ul>
      <ul class="listToastSet02">
        <li><a href="#">
          <img src="../assets/img/SlideSet/2312080002_M1.png" alt="">
          <div class="name">
            <h1>리얼 양념치킨 세트</h1>
            <p>Real Seasoned Spicy Chicken Set</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideSet/2306210035_M1.png" alt="">
          <div class="name">
            <h1>치킨 스페셜 세트</h1>
            <p>Chicken Special Set</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideSet/2306260007_M1.png" alt="">
          <div class="name">
            <h1>핫베이컨 치킨 세트</h1>
            <p>Hot Bacon Chicken Set</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideSet/2306260014_M1.png" alt="">
          <div class="name">
            <h1>햄치즈 토스트 세트</h1>
            <p>Ham Cheese Set</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideSet/2306260013_M1.png" alt="">
          <div class="name">
            <h1>햄 스페셜 토스트 세트</h1>
            <p>Ham Special Set</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideSet/2306260012_M1.png" alt="">
          <div class="name">
            <h1>베이컨 베스트 세트</h1>
            <p>Bacon Best Set</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideSet/2306280002_M1.png" alt="">
          <div class="name">
            <h1>그릴드 불갈비 세트</h1>
            <p>Grilled Bulgalbi Set</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlideSet/2306260011_M1.png" alt="">
          <div class="name">
            <h1>베이컨 포테이토 세트</h1>
            <p>Bacon Potato Set</p>
          </div>
        </a></li>
      </ul>
      </div>
      <div class="slide03" v-if="currentList === 2">
      <ul class="listToastSet">
        <li><a href="#">
          <img src="../assets/img/SlidePop/2408090002_M1.png" alt="">
          <div class="name">
            <h1>치즈 팝</h1>
            <p>Cheese Pop</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlidePop/2408090001_M1.png" alt="">
          <div class="name">
            <h1>양념치킨 팝</h1>
            <p>Seasoned Spicy Chicken Pop</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlidePop/2306210034_M1.png" alt="">
          <div class="name">
            <h1>포테이토 팝</h1>
            <p>Potato Pop</p>
          </div>
        </a></li>
      </ul>
      </div>
      <div class="slide04" v-if="currentList === 3">
      <ul class="listToastSet">
        <li><a href="#">
          <img src="../assets/img/SlidePop/2408090002_M1.png" alt="">
          <div class="name">
            <h1>아메리카노</h1>
            <p>Americano</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlidePop/2408090001_M1.png" alt="">
          <div class="name">
            <h1>아이스티</h1>
            <p>Iced Tea</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlidePop/2306210034_M1.png" alt="">
          <div class="name">
            <h1>사이다 / 제로 사이다</h1>
            <p>Cider / Zero Cider</p>
          </div>
        </a></li>
        <li><a href="#">
          <img src="../assets/img/SlidePop/2306210034_M1.png" alt="">
          <div class="name">
            <h1>콜라 / 제로 콜라</h1>
            <p>Cola / Zero Cola</p>
          </div>
        </a></li>
      </ul>
      </div>
      <p class="more"><a href="#">더보기</a></p>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      currentList: 0,
      lists : [
        {
          name: '토스트'
        },
        {
          name: '세트메뉴'
        },
        {
          name: '사이드'
        },
        {
          name: '음료'
        }
      ]
    }
  },
  methods(){
    
  }
}
</script>
<style lang="scss" scoped>
  @import '../assets/scss/Menu.scss';
</style>