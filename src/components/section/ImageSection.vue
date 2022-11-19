<template>
  <section id="imageType" class="image__wrap" :class="attr">
    <h2>이번주 판매 <em>베스트</em></h2>
    <p>모두가 사랑하는 여행지, 지금 바로 즐기세요!</p>
    <div class="image__inner" :class="layout">
      <article class="image">
        <img
          class="img img1"
          src="../../assets/img/31.jpg"
          no-repeat
          center
          alt=""
        />
        <div class="img__text">
          <h4 class="image__title">샌프란시스코 10일</h4>
          <p class="image__desc">#온천여행 #미식여행</p>
          <h5 class="image__price">1,299,300원~</h5>
        </div>
      </article>
      <article class="image">
        <img
          class="img img1"
          src="../../assets/img/32.jpg"
          no-repeat
          center
          alt=""
        />
        <div class="img__text">
          <h4 class="image__title">샌프란시스코 10일</h4>
          <p class="image__desc">#온천여행 #미식여행</p>
          <h5 class="image__price">1,299,300원~</h5>
        </div>
      </article>
      <article class="image">
        <img
          class="img img1"
          src="../../assets/img/39.jpg"
          no-repeat
          center
          alt=""
        />
        <div class="img__text">
          <h4 class="image__title">샌프란시스코 10일</h4>
          <p class="image__desc">#온천여행 #미식여행</p>
          <h5 class="image__price">1,299,300원~</h5>
        </div>
      </article>
      <article class="image">
        <img
          class="img img1"
          src="../../assets/img/40.jpg"
          no-repeat
          center
          alt=""
        />
        <div class="img__text">
          <h4 class="image__title">샌프란시스코 10일</h4>
          <p class="image__desc">#온천여행 #미식여행</p>
          <h5 class="image__price">1,299,300원~</h5>
        </div>
      </article>
      <article class="image">
        <img
          class="img img1"
          src="../../assets/img/35.jpg"
          no-repeat
          center
          alt=""
        />
        <div class="img__text">
          <h4 class="image__title">샌프란시스코 10일</h4>
          <p class="image__desc">#온천여행 #미식여행</p>
          <h5 class="image__price">1,299,300원~</h5>
        </div>
      </article>
      <article class="image">
        <img
          class="img img1"
          src="../../assets/img/36.jpg"
          no-repeat
          center
          alt=""
        />
        <div class="img__text">
          <h4 class="image__title">샌프란시스코 10일</h4>
          <p class="image__desc">#온천여행 #미식여행</p>
          <h5 class="image__price">1,299,300원~</h5>
        </div>
      </article>
      <article class="image">
        <img
          class="img img1"
          src="../../assets/img/37.jpg"
          no-repeat
          center
          alt=""
        />
        <div class="img__text">
          <h4 class="image__title">샌프란시스코 10일</h4>
          <p class="image__desc">#온천여행 #미식여행</p>
          <h5 class="image__price">1,299,300원~</h5>
        </div>
      </article>
      <article class="image">
        <img
          class="img img1"
          src="../../assets/img/38.jpg"
          no-repeat
          center
          alt=""
        />
        <div class="img__text">
          <h4 class="image__title">샌프란시스코 10일</h4>
          <p class="image__desc">#온천여행 #미식여행</p>
          <h5 class="image__price">1,299,300원~</h5>
        </div>
      </article>
    </div>
  </section>
</template>
<script>
export default {
  props: { attr: String, layout: String },
};
</script>
<style>
/* imageType */
.image__wrap {
  background-color: #f6f8fd;
}
.image__wrap em {
  color: #5e2bb9;
}
.image__inner {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
.image {
  width: 24%;
  height: 300px;
  color: 000;
  box-sizing: border-box;
}
.img__text {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  margin-top: 10px;
}
.image__title {
  font-size: 22px;
  margin-bottom: 2px;
}
.image__desc {
  color: rgb(161, 161, 161);
  font-size: 14px;
  font-weight: 300;
  margin-bottom: 10px;
  line-height: 1.5;
}
.image__price {
  font-size: 16px;
  color: black;
  letter-spacing: 1px;
}
@media (max-width: 960px) {
  .image {
    width: 32.3%;
  }
  .image:nth-child(4n) {
    display: none;
  }
  .image__title {
    font-size: 22px;
  }
}
@media (max-width: 600px) {
  .image {
    width: 49%;
  }

  .image:nth-child(3n) {
    display: none;
  }
  .image__title {
    font-size: 20px;
  }
}
</style>
