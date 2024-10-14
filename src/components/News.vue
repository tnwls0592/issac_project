<template>
  <div id="wrap" data-aos="fade-up" data-aos-duration="1500">
    <div class="inner">
      <p><img src="../assets/img/icon.png" alt=""></p>
      <h1>Isaac Toast News</h1>
      <div class="tabMenu">
      <ul class="tab">
        <li><a href="#" v-for="(tab,index) in tabs" :key="index" @click.prevent="currentTab = index" :class="{'active' : currentTab === index}">{{tab.name}}<i class="fa-solid fa-angle-right"></i></a></li>
      </ul>
      <ul class="all" v-if="currentTab === 0">
        <li><a href="#">
          <div class="img">
            <img src="../assets/img/banner/noimg.gif" alt="">
            <p>자세히보기</p>
          </div>
          <div class="text">
            <h2>[당첨자 발표] 백일장 리뷰 인증 이벤트</h2>
            <p>2024 - 04 - 30</p>
          </div>
        </a></li>
        <li><a href="#">
          <div class="img">
            <img src="../assets/img/banner/S2408261004036_1.jpg" alt="">
            <p>자세히보기</p>
          </div>
          <div class="text">
            <h2>[사연자 모집 이벤트] 든든딜리버리</h2>
            <p>2024 - 08 - 26</p>
          </div>
        </a></li>
        <li><a href="#">
          <div class="img">
            <img src="../assets/img/banner/S2408120425351_1.jpg" alt="">
            <p>자세히보기</p>
          </div>
          <div class="text">
            <h2>[매장 이벤트] 일상에 환기를 더해줄 에너지카드</h2>
            <p>2024 - 08 - 12</p>
          </div>
        </a></li>
      </ul>
      <ul class="promotion" v-if="currentTab === 1">
        <li><a href="#">
          <div class="img">
            <img src="../assets/img/banner/noimg.gif" alt="">
            <p>자세히보기</p>
          </div>
          <div class="text">
            <h2>[당첨자 발표] 우리가 함께한 달콤한 시간</h2>
            <p>2024 - 07 - 12</p>
          </div>
        </a></li>
        <li><a href="#">
          <div class="img">
            <img src="../assets/img/banner/S2406100934074_1.jpg" alt="">
            <p>자세히보기</p>
          </div>
          <div class="text">
            <h2>[프로모션] 포켓몬 랜덤 메탈 뱃지 재고 현황 및</h2>
            <p>2024 - 06 - 07</p>
          </div>
        </a></li>
        <li><a href="#">
          <div class="img">
            <img src="../assets/img/banner/noimg.gif" alt="">
            <p>자세히보기</p>
          </div>
          <div class="text">
            <h2>[참여자 선정 안내] 2024 기부 캠페인_나눔의</h2>
            <p>2024 - 05 - 23</p>
          </div>
        </a></li>
      </ul>
      <ul class="event" v-if="currentTab === 2">
        <li><a href="#">
          <div class="img">
            <img src="../assets/img/banner/S2405080933297_1.jpg" alt="">
            <p>자세히보기</p>
          </div>
          <div class="text">
            <h2>[매장 이벤트] 프렌치빵 무료 업그레이드</h2>
            <p>2024 - 05 - 08</p>
          </div>
        </a></li>
        <li><a href="#">
          <div class="img">
            <img src="../assets/img/banner/S2408261004036_1.jpg" alt="">
            <p>자세히보기</p>
          </div>
          <div class="text">
            <h2>[사연자 모집 이벤트] 든든딜리버리</h2>
            <p>2024 - 08 - 26</p>
          </div>
        </a></li>
        <li><a href="#">
          <div class="img">
            <img src="../assets/img/banner/S2408090244535_1.jpg" alt="">
            <p>자세히보기</p>
          </div>
          <div class="text">
            <h2>[신메뉴 출시 기념 이벤트] 이삭 치킨 릴레이</h2>
            <p>2024 - 08 - 09</p>
          </div>
        </a></li>
      </ul>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data(){
    return {
      currentTab: 0,
      tabs: [
        {
          name: '전체'
        },
        {
          name: '공지사항'
        },
        {
          name: '이벤트'
        }
      ]
    }
  }
}
</script>
<style lang="scss" scoped>
  @import '../assets/scss/News.scss';
</style>