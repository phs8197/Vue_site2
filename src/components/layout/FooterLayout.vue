<template>
  <footer id="footerType" :class="attr">
    <h2 className="blind">푸터 영역</h2>
    <div className="footer__inner" :class="layout">
      <div className="footer__menu">
        <div>
          <h3>해외여행</h3>
          <ul>
            <li>
              <a href="/">동남아/대만/서남아</a>
            </li>
            <li>
              <a href="/">괌/사이판/호주</a>
            </li>
            <li>
              <a href="/">유럽/아프리카</a>
            </li>
            <li>
              <a href="/">미주/중남미/하와이</a>
            </li>
            <li>
              <a href="/">일본/중국/홍콩</a>
            </li>
          </ul>
        </div>
        <div>
          <h3>국내여행</h3>
          <ul>
            <li>
              <a href="/">제주/국내여행</a>
            </li>
            <li>
              <a href="/">제주도 렌터카</a>
            </li>
            <li>
              <a href="/">단독 여행문의</a>
            </li>
          </ul>
        </div>
        <div>
          <h3>항공/숙박</h3>
          <ul>
            <li>
              <a href="/">항공권</a>
            </li>
            <li>
              <a href="/">숙박</a>
            </li>
            <li>
              <a href="/">최저가 검색</a>
            </li>
            <li>
              <a href="/">최저 특가</a>
            </li>
          </ul>
        </div>
        <div>
          <h3>투어/입장권</h3>
          <ul>
            <li>
              <a href="/">국내</a>
            </li>
            <li>
              <a href="/">동남아/중국/일본</a>
            </li>
            <li>
              <a href="/">유럽/중동</a>
            </li>
            <li>
              <a href="/">미주</a>
            </li>
          </ul>
        </div>
        <div>
          <h3>허니문/골프</h3>
          <ul>
            <li>
              <a href="/">허니문</a>
            </li>
            <li>
              <a href="/">골프</a>
            </li>
            <li>
              <a href="/">단독 여행문의</a>
            </li>
          </ul>
        </div>
      </div>
      <div className="footer__right">
        2022 Webstoryboy. Portfolio is Power
        <br />
        All rights reserved.
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  props: { attr: String, layout: String },
};
</script>
<style>
.footer__menu {
  display: flex;
  margin-bottom: 70px;
  justify-content: center;
}
.footer__menu > div {
  width: 20%;
}
.footer__menu h3 {
  font-size: 18px;
  margin-bottom: 20px;
}
.footer__menu li a {
  font-size: 14px;
  color: #666;
  margin-bottom: 10px;
  display: block;
}
.footer__right {
  border-top: 1px solid #d9d9d9;
  text-align: center;
  padding-top: 40px;
  color: #666;
  line-height: 1.5;
}

@media (max-width: 960px) {
  .footer__menu {
    display: none;
  }
  .footer__right {
    padding-top: 0;
    border-top: 0;
  }
  .footer__wrap {
    padding: 40px 0;
  }
}
</style>
