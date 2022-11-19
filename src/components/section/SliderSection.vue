<template>
  <swiper
    :modules="modules"
    :slides-per-view="1"
    :space-between="50"
    navigation
    :pagination="{ clickable: true }"
    :scrollbar="{ draggable: true }"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
  >
    <swiper-slide
      v-bind:style="{
        backgroundImage: 'url(../../assets/img/31.jpg)',
        backgroundSize: 'cover',
        backgroundRepeat: 'no-repeat',
        backgroundPosition: 'center',
      }"
    >
      <div class="slide__txt">
        <span>699,000원~</span>
        <h1>샌프란시스코 6박 7일</h1>
        <p>#온천여행 #미국 #6박 7일</p>
        <button>자세히 보기</button>
      </div>
    </swiper-slide>

    <swiper-slide
      v-bind:style="{
        backgroundImage: 'url(../../assets/img/32.jpg)',
        backgroundSize: 'cover',
        backgroundRepeat: 'no-repeat',
        backgroundPosition: 'center',
      }"
    >
      <div className="slide__txt">
        <span>1,499,000원~</span>
        <h1>캐나다 동부 7박 9일</h1>
        <p>#온천여행 #미국 #6박 7일</p>
        <button>자세히 보기</button>
      </div>
    </swiper-slide>

    <swiper-slide
      v-bind:style="{
        backgroundImage: 'url(../../assets/img/33.jpg)',
        backgroundSize: 'cover',
        backgroundRepeat: 'no-repeat',
        backgroundPosition: 'center',
      }"
    >
      <div className="slide__txt">
        <span>1,999,000원~</span>
        <h1>호주/뉴질랜드 6박 7일</h1>
        <p>#온천여행 #미국 #6박 7일</p>
        <button>자세히 보기</button>
      </div>
    </swiper-slide>
  </swiper>
</template>
<script>
// import Swiper core and required modules
import { Navigation, Pagination, Scrollbar, A11y } from "swiper";

// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";
import "swiper/css/navigation";
import "swiper/css/pagination";
import "swiper/css/scrollbar";

// Import Swiper styles
export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    const onSwiper = (swiper) => {
      console.log(swiper);
    };
    const onSlideChange = () => {
      console.log("slide change");
    };
    return {
      onSwiper,
      onSlideChange,
      modules: [Navigation, Pagination, Scrollbar, A11y],
    };
  },
};
</script>
<style>
.swiper {
  height: 800px;
}
.slide__txt {
  position: absolute;
  top: 20%;
  left: 5%;
  color: white;
  z-index: 2;
  background-color: rgba(0, 0, 0, 0.5);
  width: 500px;
  height: 300px;
  padding: 20px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}
.slide__txt span {
  margin-left: 1%;
}
.slide__txt h1 {
  font-size: 50px;
  font-weight: 600;
  margin-top: 20px;
}
.slide__txt p {
  margin-top: 30px;
}
.slide__txt button {
  margin-top: 120px;
  font-size: 16px;
  padding: 10px 30px;
  font-family: "GmarketSans";
  background-color: #5e2bb9;
  color: white;
}
@media (max-width: 960px) {
  .swiper {
    height: 600px;
  }
  .slide__txt {
    width: 400px;
    height: 150px;
  }
  .slide__txt h1 {
    font-size: 30px;
    margin-top: 10px;
  }
  .slide__txt p {
    display: none;
  }
  .slide__txt button {
    margin-top: 20px;
    background: none;
    padding: 0;
    margin-left: 0;
    border-bottom: 1px solid white;
  }
}
@media (max-width: 600px) {
  .slide__txt {
    width: 400px;
    height: 100px;
  }
  .swiper {
    height: 400px;
  }
  .slide__txt h1 {
    margin-top: 0;
  }
  .slide__txt span {
    display: none;
  }
}
</style>
