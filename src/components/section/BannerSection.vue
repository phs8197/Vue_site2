<template>
  <section id="bannerType" :class="fonts">
    <h2 class="blind">배너 영역</h2>
    <div class="banner__inner">
      <h3 class="title"><em>하나투어</em> 유투브</h3>
      <p class="desc">
        지금 하나투어 유투브를 구독하고,
        <br />
        인스타로 인증하면 선착순으로 <em>5% 할인쿠폰</em>을 드립니다!
      </p>
      <button>구독하기</button>
    </div>
  </section>
</template>
<script>
export default {
  props: {
    fonts: String,
  },
};
</script>
<style>
.banner__inner {
  background-image: url(../../assets/img/502.svg);
  height: 250px;
  background-repeat: no-repeat;
  background-position: center;
  text-align: start;
  padding: 120px 200px;
  color: #fff;
}
.banner__inner .title {
  color: #000;
  font-size: 40px;
  font-weight: 600;
  line-height: 1;
  margin-bottom: 20px;
}
.banner__inner em {
  color: #5e2bb9;
}
.banner__inner .desc {
  color: #000;
  font-size: 20px;
  line-height: 1.5;
  font-weight: 300;
  margin-bottom: 70px;
}
.banner__inner button {
  background-color: #5e2bb9;
  color: #fff;
  font-size: 16px;
  padding: 10px 30px;
  border-radius: 2px;
}

@media (max-width: 960px) {
  .banner__inner {
    padding: 100px 0;
    margin-left: 40px;
  }
}

@media (max-width: 600px) {
  .banner__inner {
    background-image: none;
    height: 200px;
    margin-left: 20px;
  }
  .banner__inner .title {
    font-size: 30px;
    margin-bottom: 20px;
  }
  .banner__inner .desc {
    font-size: 16px;
    margin-bottom: 40px;
  }
}
</style>
