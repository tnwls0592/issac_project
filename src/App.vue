<template>
  <Header />
  <main-section />
  <Footer />
</template>

<script>
import Header from './components/Header.vue';
import MainSection from './components/MainSection.vue';
import Footer from './components/Footer.vue';
export default {
  components: {
    Header,
    MainSection,
    Footer
  }
}
</script>

<style>
  @font-face {
    font-family: 'LOTTERIACHAB';
    src: url('https://fastly.jsdelivr.net/gh/projectnoonnu/noonfonts_2302@1.0/LOTTERIACHAB.woff2') format('woff2');
    font-weight: normal;
    font-style: normal;
  }
  @font-face {
    font-family: 'Pretendard-Regular';
    src: url('https://fastly.jsdelivr.net/gh/Project-Noonnu/noonfonts_2107@1.1/Pretendard-Regular.woff') format('woff');
    font-weight: 400;
    font-style: normal;
  }
  body {
    font-family: 'Pretendard-Regular';
  }
  li {
    list-style: none;
  }
  a {
    color: inherit;
    text-decoration: none;
  }
</style>
