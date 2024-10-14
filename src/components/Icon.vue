<template>
  <div id="wrap">
    <img src="../assets/img/egg.png" alt="" class="egg">
    <img src="../assets/img/bread.png" alt="" class="bread">
    <img src="../assets/img/meet.png" alt="" class="meet">
    <img src="../assets/img/chesse.png" alt="" class="chesse">
    <img src="../assets/img/cucomber.png" alt="" class="cucomber">
    <img src="../assets/img/bg.png" alt="" class="bg">
  </div>
</template>
<script>
export default {
  
}
</script>
<style lang="scss" scoped>
  #wrap {
    opacity: .6;
    position: relative;
    z-index: -1;
    img {
      transition: .5s;
    :hover {
      transform: scale(1.2);
    }
    }
    .egg {
      animation: rotate 10s infinite linear;
      width: 150px;
      position: fixed;
      top: 200px; left: 200px;
      z-index: -1;
    }
    .bread {
      animation: rotate 13s infinite linear;
      width: 150px;
      position: fixed;
      top: 370px; right: 500px;
      z-index: -1;
    }
    .meet {
      animation: rotate 12s infinite linear;
      width: 150px;
      position: fixed;
      top: 600px; left: 100px;
      z-index: -1;
    }
    .cucomber {
      animation: rotate 8s infinite linear;
      width: 150px;
      position: fixed;
      top: 350px; left: 500px;
      z-index: -1;
    }
    .chesse {
      animation: rotate 11s infinite linear;
      width: 150px;
      position: fixed;
      top: 150px; right: 300px;
      z-index: -1;
    }
    .bg {
      animation: rotate 9s infinite linear;
      width: 150px;
      position: fixed;
      top: 530px; right: 200px;
      
      z-index: -1;
    }
  }
  @keyframes rotate {
    0% {transform: rotate(0) scale(1);}
    50% {transform: rotate(180deg) scale(.7);}
    100% {transform: rotate(360deg) scale(1);}
  }
</style>