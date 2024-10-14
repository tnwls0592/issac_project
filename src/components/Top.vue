<template>
  <div class="goTop">
      <ul>
        <li @click="top"><i class="fa-solid fa-chevron-up"></i>TOP</li>
        <li><i class="fa-brands fa-instagram"></i>인스타그램</li>
        <li><i class="fa-solid fa-headset"></i>고객문의</li>
        <li><i class="fa-regular fa-comments"></i>제휴/제안</li>
        <li><i class="fa-solid fa-store"></i>가맹상담<br>1833-9299</li>
      </ul>
    </div>
</template>
<script>
export default {
  methods: {
    top(){
      window.scrollTo({top:0,behavior:'smooth'});
    }
  }
}
</script>
<style lang="scss" scoped>
  .goTop {
    position: fixed;
    top: 50%; right: 50px;
    z-index: 50;
    transform: translate(0,-50%);
    ul {
      border-radius: 10px;
      background: rgba(255, 255, 255,.8);
      color: #888888;
      border: 1px solid #ccc;
      box-shadow: 2px 2px 2px #eee;
      transition: .5s;
      li {
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 80px;
        height: 80px;
        font-size: 13px;
        font-weight: 700;
        text-align: center;
        transition: .5s;
        i {
          font-size: 20px;
          padding: 10px 0;
          margin-top: 5px;
        }
      }
      li:hover {
        color: #ff281e;
      }
      li:last-child {
        i {
          font-size: 20px;
          padding: 10px 0;
          margin: 0;
        }
      }
    }
    ul:hover {
      border: 1px solid #ff281e;
    }
  }
</style>