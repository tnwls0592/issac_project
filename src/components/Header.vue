<template>
  <div id="wrap">
    <div class="inner">
      <div class="logo">
        <img src="../assets/img/logo.svg" alt="">
      </div>
      <div class="menu">
        <ul class="main_menu">
          <li @mouseenter="on=true" @mouseleave="on=false"><a href="#">브랜드</a>
            <div class="sub_menu" v-show="on">
              <div class="inner">
                <ul>
                  <li><a href="#">이삭토스트</a></li>
                  <li><a href="#">CEO 인사말</a></li>
                  <li><a href="#">연혁</a></li>
                </ul>
                <ul>
                  <li><a href="#"></a></li>
                </ul>
                <ul>
                  <li><a href="#"></a></li>
                </ul>
                <ul>
                  <li><a href="#">공지사항</a></li>
                  <li><a href="#">이벤트뉴스</a></li>
                  <li><a href="#">기부 캠페인</a></li>
                  <li><a href="#">고객 리뷰</a></li>
                </ul>
                <ul>
                  <li><a href="#">매장 칭찬하기</a></li>
                  <li><a href="#">FAQ</a></li>
                  <li><a href="#">고객 문의</a></li>
                  <li><a href="#">제휴/제안</a></li>
                </ul>
                <ul>
                  <li><a href="#">가맹 상담 신청</a></li>
                  <li><a href="#">비용 및 절차</a></li>
                  <li><a href="#">교육프로그램</a></li>
                  <li><a href="#">인테리어</a></li>
                </ul>
              </div>
            </div>
          </li>
          <li @mouseenter="on=true" @mouseleave="on=false"><a href="#">메뉴</a></li>
          <li @mouseenter="on=true" @mouseleave="on=false"><a href="#">사회공헌</a></li>
          <li @mouseenter="on=true" @mouseleave="on=false"><a href="#">커뮤니티</a></li>
          <li @mouseenter="on=true" @mouseleave="on=false"><a href="#">고객게시판</a></li>
          <li @mouseenter="on=true" @mouseleave="on=false"><a href="#">가맹안내</a></li>
        </ul>
      </div>
        <i class="fa-solid fa-bars"></i>
    </div>
  </div>
</template>
<script>
export default {
  data(){
    return {
      on:false
    }
  }
}
</script>
<style lang="scss" scoped>
  @import '../assets/scss/Header.scss';
</style>