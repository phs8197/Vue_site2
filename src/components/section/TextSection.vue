<template>
  <section id="textType" class="text__wrap" :class="attr">
    <div class="text__container" :class="layout">
      <div class="text__text">
        <span class="mb70">HANA TOUR</span>
        <h2 class="mb40">여행 가실래요?</h2>
        <p class="mb70">
          여행이 일상화된 요즘 시대,
          <br />
          포기했던 여행을 다시 꿈꾸고,
          <br />
          당신의 세계가 넓어질 수 있도록
          <br />
          새로운 하나투어가 함께 하겠습니다.
        </p>
      </div>
      <div class="text__innner">
        <div class="text t2">
          <h3 class="text__title">여행을 만듭니다.</h3>
          <p class="text__desc">
            익숙하지만 색다른 이야기를 모든 이들의
            <br />
            여행의 꿈을 실현해드립니다.
          </p>
          <a class="text_btn" href="/"> 더보기 </a>
        </div>
        <div class="text t3">
          <h3 class="text__title">문화를 만듭니다.</h3>
          <p class="text__desc">
            여행을 넘어, 즐기고, 먹고 머무는 곳까지
            <br />더 큰 행복을 위해 우리는 문화를 만듭니다.
          </p>
          <a class="text_btn" href="/"> 더보기 </a>
        </div>
        <div class="text t5">
          <h3 class="text__title">행복을 만듭니다.</h3>
          <p class="text__desc">
            고객에게 여행을 통한 행복을 선사하고,
            <br />
            고객의 행복을 느끼며,
            <br />
            또다른 행복을 만듭니다.
          </p>
          <a class="text_btn" href="/"> 더보기 </a>
        </div>
        <div class="text t6">
          <h3 class="text__title">고객을 중심으로</h3>
          <p class="text__desc">
            고객을 중심으로 여행의 시작부터
            <br />
            끝까지 모든 것을 함께 할 수 있도록
            <br />
            하나투어가 함께 하겠습니다.
          </p>
          <a class="text_btn" href="/"> 더보기 </a>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  props: { attr: String, layout: String },
};
</script>
<style>
.text__wrap {
  background-color: #f6f8fd;
}
.text__container {
  display: flex;
}
.text__text {
  width: 30%;
}
.text__text span {
  background-color: #5e2bb9;
  color: white;
  font-size: 14px;
  padding: 3px 10px;
  border-radius: 10px;
}
.text__text h2 {
  font-size: 40px;
  font-weight: 600;
  text-align: flex-start;
  line-height: 1.1;
  margin-top: 20px;
}
.text__text p {
  line-height: 1.5;
}
.text__innner {
  width: 70%;
  display: flex;
  flex-wrap: wrap;
  justify-content: flex-end;
}
.text {
  width: 48%;
  margin-bottom: 2%;
  padding: 20px 0 20px 20px;
  box-sizing: border-box;
  border-radius: 10px;
  transition: background 0.4s;
}
.text:hover {
  background: #f5f5f5;
}
.text__title {
  font-size: 24px;
  line-height: 1;
  margin-bottom: 30px;
  white-space: nowrap;
  text-overflow: ellipsis;
  position: relative;
  padding-top: 75px;
}
.text__title::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  width: 60px;
  height: 60px;
  background: url(../../assets/img/text_icon.svg);
}
.text.t1 .text__title::before {
  background-position: 0 0;
}
.text.t2 .text__title::before {
  background-position: -60px 0;
}
.text.t3 .text__title::before {
  background-position: -120px 0;
}
.text.t4 .text__title::before {
  background-position: -180px 0;
}
.text.t5 .text__title::before {
  background-position: -240px 0;
}
.text.t6 .text__title::before {
  background-position: -300px 0;
}
.text__desc {
  font-size: 18px;
  font-weight: 300;
  line-height: 1.4;
  /* overflow: hidden;
    text-overflow: ellipsis;
    display: -webkit-box;
    -webkit-line-clamp: 3;
    -webkit-box-orient: vertical; */
  color: #666;
  margin-bottom: 20px;
}
.text_btn {
  font-size: 16px;
  line-height: 1;
  text-decoration: underline;
  text-underline-position: under;
  color: #666;
}

@media (max-width: 960px) {
  .text__container {
    width: 100%;
    margin: 0 auto;
    padding: 0 20px;
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 0;
  }
  .text {
    padding: 0;
  }
  .text__text {
    width: 100%;
    text-align: center;
  }
  .text__text p {
    display: none;
  }
  .text__inner {
    width: 100%;
  }
  .text__desc {
    display: none;
  }
}
@media (max-width: 600px) {
  .text__wrap {
    display: none;
  }
}
</style>
