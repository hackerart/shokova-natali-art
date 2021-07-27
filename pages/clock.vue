<template>
  <div class="app">
    <Navbar />
    <div class="mainHeadline-container container-fluid px-0">
      <div class="position-absolute mainHeadline-backgroundImg mainHeadline-backImgLine">
        <div class="mainHeadline-backgroundImg-img-1">
          <img src="../static/img/theMainHeadline/clock/1.png" alt="">
        </div>
        <div class="mainHeadline-backgroundImg-img-2">
          <img src="../static/img/theMainHeadline/clock/2.png" alt="">
        </div>
      </div>
      <div class="position-absolute mainHeadline-backgroundImg background-position-right">
        <div class="mainHeadline-backgroundImg-img-1-reverse">
          <img src="../static/img/theMainHeadline/clock/3.png" alt="">
        </div>
      </div>
      <div class="mainHeadline-title d-flex flex-column align-items-center">
        <h1>Изготовление часов <br> из эпоксидной смолы под заказ.</h1>
        <p>Вы можете заказать часы исключительно под свой интерьер, как по цветам, так и по материалам.</p>
        <button>
          Записаться на консультацию
        </button>
      </div>
    </div>
    <div class="infoWork-container d-flex align-items-center justify-content-between">
      <div class="info-main-container border-0 pl-0">
        <h2>7 день</h2>
        <p>Уходит в среднем на написание картины.</p>
      </div>
      <div class="info-main-container">
        <h2 class="text-center">30 см</h2>
        <p>Минимальный размер, с которым мы работаем.</p>
      </div>
      <div class="info-main-container border-0 pr-0">
        <h2>от 3000 ₽</h2>
        <p>Минимальная сумма заказа</p>
      </div>
    </div>
    <div class="picture-scroll-container">
      <div class="scroll-carousel-container">
        <div class="slider">
          <div class="cursor"></div>
          <div class="slider__wrapper" :style="`left: ${padding}px`">
            <div class="slider__block slider__block_left">
              <img class="slider__img slider__block_margin" src="../static/img/theScrollText/clock/1.png" alt="" />

              <div class="slider__img-block slider__block_margin">
                <img class="slider__img" src="../static/img/theScrollText/clock/2.png" alt="" />
                <img class="slider__img" src="../static/img/theScrollText/clock/3.png" alt="" />
              </div>
            </div>

            <div class="slider__block slider__block_middle">
              <img class="slider__img slider__block_margin" src="../static/img/theScrollText/clock/4.png" alt="" />

              <div class="slider__img-block slider__block_margin">
                <img class="slider__img" src="../static/img/theScrollText/clock/5.png" alt="" />
                <img class="slider__img" src="../static/img/theScrollText/clock/6.png" alt="" />
              </div>

              <img class="slider__img slider__block_margin" src="../static/img/theScrollText/clock/7.png" alt="" />

              <div class="slider__img-block slider__block_margin">
                <img class="slider__img" src="../static/img/theScrollText/clock/2.png" alt="" />
                <img class="slider__img" src="../static/img/theScrollText/clock/3.png" alt="" />
              </div>

              <img class="slider__img slider__block_margin" src="../static/img/theScrollText/clock/4.png" alt="" />
            </div>

            <div class="slider__block slider__block_right">
              <img class="slider__img slider__block_margin" src="../static/img/theScrollText/clock/7.png" alt="" />

              <div class="slider__img-block slider_margin">
                <img class="slider__img" src="../static/img/theScrollText/clock/5.png" alt="" />
                <img class="slider__img" src="../static/img/theScrollText/clock/6.png" alt="" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="carousel-container">
      <div class="d-flex justify-content-between align-items-end desc-carousel">
        <div>
          <h4>Мы изготавливаем столы в современных техниках.</h4>
          <p class="desc-carousel-text">Техники в основном зависят от элементов которые используются при создании столов.</p>
        </div>
        <div class="d-flex align-items-center desc-carousel-instruction">
          <img src="../static/img/theCarousel/cursor.png" alt="">
          <p>Протяните контент по горизонтали</p>
        </div>
      </div>
      <client-only>
        <carousel v-bind="options" class="carousel-main-container">
          <slide class="img-wrapper">
            <img src="../static/img/theCarousel/clock/1.png" />
          </slide>
          <slide class="img-wrapper">
            <img src="../static/img/theCarousel/clock/2.png" />
          </slide>
          <slide class="img-wrapper">
            <img src="../static/img/theCarousel/clock/3.png" />
          </slide>
        </carousel>
      </client-only>
    </div>
    <div class="banner-container">
      <div class="main-banner-container d-flex align-items-center">
        <div class="main-banner-title">
          <h2 class="mb-0">Обрабатываем часы специальным лаком.</h2>
        </div>
        <div class="main-banner-text">
          <p>Все часы обрабатываются специальным лаком, который защищает их от влажности и выгорания. Можно протирать влажной тряпкой.</p>
        </div>
      </div>
    </div>
    <div class="process-container" id="process">
      <h2>Процесс работы.</h2>
      <b-list-group horizontal class="list-group-container d-flex flex-wrap">
        <b-list-group-item class="d-flex"><span>01</span> <p class="mb-0">Оставляете заявку</p></b-list-group-item>
        <b-list-group-item class="d-flex"><span>02</span> <p class="mb-0">Наш дизайнер бесплатно поможет с выбором декора под ваш интерьер</p></b-list-group-item>
        <b-list-group-item class="d-flex"><span>03</span> <p class="mb-0">Наши художники начинают работу</p></b-list-group-item>
        <b-list-group-item class="d-flex"><span>04</span> <p class="mb-0">По ходу процесса художники согласуют промежуточные результаты</p></b-list-group-item>
        <b-list-group-item class="d-flex"><span>05</span> <p class="mb-0">Заказ упаковыват и доставляют</p></b-list-group-item>
        <b-list-group-item class="d-flex"><p class="bold-text mb-0">Картины создают уют, устраняют визуальный дисбаланс, а также подчёркивают статус.</p></b-list-group-item>
      </b-list-group>
    </div>
    <div class="picture-scroll-container pb-0">
      <div class="scroll-carousel-container">
        <div class="slider">
          <div class="cursor"></div>
          <div class="slider__wrapper" :style="`left: ${padding2}px`">
            <div class="slider__block slider__block_left">
              <img class="slider__img slider__block_margin" src="../static/img/theScrollText/clock/2/1.png" alt="" />

              <div class="slider__img-block slider__block_margin">
                <img class="slider__img" src="../static/img/theScrollText/clock/2/2.png" alt="" />
                <img class="slider__img" src="../static/img/theScrollText/clock/2/3.png" alt="" />
              </div>
            </div>

            <div class="slider__block slider__block_middle">
              <img class="slider__img slider__block_margin" src="../static/img/theScrollText/clock/2/4.png" alt="" />

              <div class="slider__img-block slider__block_margin">
                <img class="slider__img" src="../static/img/theScrollText/clock/2/5.png" alt="" />
                <img class="slider__img" src="../static/img/theScrollText/clock/2/6.png" alt="" />
              </div>

              <img class="slider__img slider__block_margin" src="../static/img/theScrollText/clock/2/7.png" alt="" />

              <div class="slider__img-block slider__block_margin">
                <img class="slider__img" src="../static/img/theScrollText/clock/2/2.png" alt="" />
                <img class="slider__img" src="../static/img/theScrollText/clock/2/3.png" alt="" />
              </div>

              <img class="slider__img slider__block_margin" src="../static/img/theScrollText/clock/2/4.png" alt="" />
            </div>

            <div class="slider__block slider__block_right">
              <img class="slider__img slider__block_margin" src="../static/img/theScrollText/clock/2/7.png" alt="" />

              <div class="slider__img-block slider_margin">
                <img class="slider__img" src="../static/img/theScrollText/clock/2/5.png" alt="" />
                <img class="slider__img" src="../static/img/theScrollText/clock/2/6.png" alt="" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <TheConsult />
    <Footer />
  </div>
</template>

<script>
import TheInfoWork from "../components/TheInfoWork";
export default {
  components: {
    TheInfoWork
  },
  data: () => ({
    padding: 0,
    padding2: 0,
    options: {
      autoplay: true,
      paginationEnabled: false,
      scrollPerPage: false,
      perPage: 3,
    },
  }),
  created() {
    if(process.browser) {
      window.addEventListener('scroll', this.handleScroll)
    }
  },
  destroyed() {
    if (process.browser) {
      window.removeEventListener('scroll', this.handleScroll)
    }
  },
  methods: {
    handleScroll() {
      console.log('test', window.pageYOffset)
      this.padding = (window.pageYOffset - 450) * 0.5
      this.padding2 = (window.pageYOffset - 3395) * 0.5
    }
  },
  mounted() {
    if (this.$vssWidth < 440) {
      this.options.perPage = 1.5
      this.options.autoplay = false
    }
  }
}
</script>

<style lang="scss" scoped>
.app {
  background-color: #FFF8EF;
}
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Jost&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Jost:wght@600&disp lay=swap');
.mainHeadline-container {
  padding: 7.5rem 0 8.6rem;
  margin-bottom: 12.5rem;
  @media screen and (max-width: 440px){
    padding: 1.875rem 1rem 6.25rem!important;
    margin-bottom: 0;
  }
  .background-position-right {
    right: 0;
    display: flex;
    flex-direction: column;
    align-items: flex-end;
  }
  .mainHeadline-backImgLine {
    background-image: url("./static/img/theMainHeadline/picture/back.png");
    background-repeat: no-repeat;
    background-position: left bottom;
  }
  .mainHeadline-backgroundImg {
    .mainHeadline-backgroundImg-img {
      &-1 {
        margin-bottom: 5rem;
      }
      &-2 {
        margin-left: 22.5rem;
      }
      &-1-reverse {
        z-index: 0;
      }
      @media screen and (max-width: 440px){
        &-1 {
          display: none;
        }
        &-2-reverse {
          display: none;
        }
        &-2 {
          display: none;
        }
        &-1-reverse {
          display: none;
        }
      }
      @media screen and (max-width: 768px) and (min-width: 441px){
        &-1 {
          display: none;
        }
        &-2-reverse {
          display: none;
        }
        &-2 {
          margin-left: 0;
          margin-top: 240%;
        }
        &-1-reverse {
          margin: 0;
        }
      }
      @media screen and (max-width: 1001px) and (min-width: 900px) {
        &-2 {
          margin-left: 0;
          margin-top: 330%!important;
        }
      }
      @media screen and (max-width: 1100px) and (min-width: 769px) {
        &-1 {
          display: none;
        }
        &-2-reverse {
          display: none;
        }
        &-2 {
          margin-left: 0;
          margin-top: 270%;
        }
        &-1-reverse {
          margin: 0;
        }
      }
      @media screen and (max-width: 1441px) and (min-width: 1300px) {
        &-2 {
          margin-left: 13.5rem;
        }
        &-1-reverse {
          margin-bottom: 5rem;
          margin-right: 13.5rem;
        }
      }
    }
  }
  .mainHeadline-title {
    h1 {
      font-size: 3.75rem;
      font-family: Playfair Display,serif;
      line-height: 150%;
      text-transform: uppercase;
      color: #2F1D07;
      width: 45%;
      text-align: center;
      margin-bottom: 1.875rem;
      z-index: 20;
      @media screen and (max-width: 1441px) and (min-width: 1300px) {
        width: 58%;
        z-index: 2;
      }
      @media screen and (max-width: 1100px) and (min-width: 769px) {
        width: 80%;
        z-index: 2;
      }
      @media screen and (max-width: 1001px) and (min-width: 900px) {
        width: 85%!important;
        z-index: 2;
      }
      @media screen and (max-width: 768px) and (min-width: 441px){
        font-size: 3.125rem;
        width: 90%;
        z-index: 2;
      }
      @media screen and (max-width: 440px){
        font-size: 1.5625rem;
        width: 78%;
      }
    }
    p {
      color: #2F1D07;
      font-size: 1rem;
      font-family: Jost,serif;
      line-height: 150%;
      text-align: center;
      width: 19.5%;
      margin-bottom: 1.875rem;
      @media screen and (max-width: 1441px) and (min-width: 1300px) {
        width: 25.5%;
      }
      @media screen and (max-width: 1100px) and (min-width: 769px) {
        width: 34.5%;
      }
      @media screen and (max-width: 768px) and (min-width: 441px){
        width: 46.5%;
      }
      @media screen and (max-width: 440px){
        width: 75%;
      }
    }
    button {
      background-color: #E1CAAF;
      color: #2F1D07;
      padding: 1.25rem 1.875rem;
      font-size: 1rem;
      font-family: Jost, serif;
      font-weight: 600;
      line-height: 150%;
      border: none;
      &:hover {
        background-color: #2F1D07;
        color: #FFF8EF;
        transition: .3s;
      }
      @media screen and (max-width: 440px){
        width: 100%;
      }
    }
  }
}
.infoWork-container {
  padding: 0 26.25rem;
  .info-main-container {
    padding: 0 5rem;
    border: 1px solid #E1CAAF;
    border-top: 0;
    border-bottom: 0;
    width: 100%;
    h2 {
      font-family: PlayFair, serif;
      color: #2F1D07;
      font-size: 3.75rem;
      line-height: 150%;
    }
    p {
      color: #2F1D07;
      font-size: 1rem;
      line-height: 150%;
      font-family: Jost, serif;
    }
  }
}
.picture-scroll-container {
  padding: 12.5rem 0;
  .scroll-carousel-container {
    @media screen and (max-width: 440px){
      padding-top: 6.25rem;
    }
    .scroll-carousel-desc-container {
      padding: 0 22.5rem;
      margin-bottom: 6.25rem;
      @media screen and (max-width: 1441px) and (min-width: 1300px) {
        padding: 0 11.25rem;
      }
      @media screen and (max-width: 1100px) and (min-width: 769px) {
        padding: 0 1.875rem;
      }
      @media screen and (max-width: 768px) and (min-width: 441px){
        padding: 0 1.25rem;
      }
      @media screen and (max-width: 440px){
        padding: 0 1rem;
        margin-bottom: 3.125rem;
      }
      p {
        font-family: Jost, serif;
        font-size: 1rem;
        line-height: 150%;
        color: #2F1D07;
        width: 30%;
        text-align: center;
        margin-bottom: 0;
        @media screen and (max-width: 1100px) and (min-width: 769px) {
          width: 40%;
        }
        @media screen and (max-width: 768px) and (min-width: 441px){
          width: 50%;
        }
        @media screen and (max-width: 440px){
          width: 70%;
        }
      }
      h1 {
        font-family: PlayFair, serif;
        text-transform: uppercase;
        font-size: 3.75rem;
        line-height: 150%;
        color: #2F1D07;
        margin-bottom: 1.875rem;
        text-align: center;
        width: 60%;
        @media screen and (max-width: 1100px) and (min-width: 769px) {
          width: 80%;
        }
        @media screen and (max-width: 768px) and (min-width: 441px){
          font-size: 3.125rem;
          width: 80%;
        }
        @media screen and (max-width: 440px){
          font-size: 1.5625rem;
          margin-bottom: 1.5625rem;
          width: 80%;
        }
      }
    }
  }
  .container {
    max-width: 1110px;
    margin: 0 auto;
    padding: 0 15px;
  }
  .slider {
    position: relative;
    width: 100%;
    height: 540px;
    overflow: hidden;
    &__wrapper {
      display: flex;
      position: absolute;
      left: 0;
    }
    &__img {
    }
    &__block {
      display: flex;

      &_margin {
        margin-right: 100px;

        &:last-child {
          margin-right: 0px;
        }
      }
      &_left {
        width: 680px;
        position: absolute;
        top: 0;
        left: -780px;
      }
      &_middle {
        position: absolute;
        top: 0;
        left: 0;
        width: 1920px;
      }
      &_right {
        position: absolute;
        top: 0;
        left: 2020px;
        width: 680px;
      }
    }
    &__img-block {
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }
  }
}
.carousel-container {
  padding: 0 22.5rem;
  @media screen and (max-width: 1441px) and (min-width: 1300px) {
    padding: 0 11.25rem;
  }
  @media screen and (max-width: 1100px) and (min-width: 769px){
    padding: 0 1.875rem;
    .carousel-main-container {
      img {
        max-width: 15.375rem;
      }
    }
  }
  @media screen and (max-width: 768px) and (min-width: 441px){
    padding: 0 1.25rem;
    .carousel-main-container {
      img {
        max-width: 13rem;
      }
    }
  }
  @media screen and (max-width: 440px){
    padding: 0;
    .carousel-main-container {
      img {
        max-width: 13rem;
      }
    }
  }
  .desc-carousel {
    margin-bottom: 5rem;
  }
  h4 {
    color: #2F1D07;
    font-family: PlayFair, serif;
    font-size: 2.5rem;
    line-height: 150%;
    text-transform: uppercase;
    width: 65%;
    margin-bottom: 1.875rem;
    @media screen and (max-width: 1100px) and (min-width: 769px){
      width: 60%;
    }
    @media screen and (max-width: 768px) and (min-width: 441px){
      font-size: 3.125rem;
      width: 60%;
    }
    @media screen and (max-width: 440px){
      font-size: 1.5rem;
      margin-bottom: 3.125rem;
      width: 60%;
    }
  }
  .desc-carousel-text {
    width: 40%;
  }
  p {
    color: #2F1D07;
    font-family: Jost, serif;
    font-size: 1rem;
    line-height: 150%;
    margin-bottom: 0;
  }
  .desc-carousel-instruction {
    img {
      margin-right: 1rem;
    }

  }
  .carousel-main-container {
    @media screen and (max-width: 440px){
      .VueCarousel-inner {
        flex-basis: 260px!important;
      }
      .VueCarousel-slide {
        &:first-child {
          text-align: start;
        }
        &:nth-child(2) {
          text-align: start!important;
        }
        &:last-child {
          text-align: start!important;
        }
      }
    }
    .VueCarousel-slide {
      &:nth-child(2) {
        text-align: center;
      }
      &:last-child {
        text-align: right;
      }
    }
  }
}
.banner-container {
  padding: 12.5rem 11.25rem;
  background-image: url("../static/img/theBanner/back2.png");
  background-repeat: no-repeat;
  background-position: left 2% bottom;
  @media screen and (max-width: 1441px) and (min-width: 1300px) {
    background-position: left 3% bottom;
  }
  @media screen and (max-width: 1100px) and (min-width: 415px){
    background-image: none;
    padding: 9.375rem 0;
  }
  @media screen and (max-width: 415px) {
    background-image: none;
    padding: 6.25rem 0 6.25rem 0;
  }
  .main-banner-container {
    padding: 6.25rem 11.25rem;
    background-color: #F3E6D7;
    @media screen and (max-width: 1441px) and (min-width: 1300px) {
      padding: 6.25rem 3.25rem;
    }
    @media screen and (max-width: 1100px) and (min-width: 769px){
      padding: 6.25rem 1.875rem;
    }
    @media screen and (max-width: 768px) and (min-width: 415px){
      padding: 3.125rem 1.875rem;
    }
    @media screen and (max-width: 440px) {
      flex-direction: column;
      padding: 3.125rem 1rem;
    }
    .main-banner-title {
      width: 50%;
      @media screen and (max-width: 1441px) and (min-width: 1300px) {
        width: 64%;
      }
      @media screen and (max-width: 1100px) and (min-width: 769px){
        width: 48%;
      }
      @media screen and (max-width: 440px) {
        width: 100%;
      }
      h2 {
        color: #2F1D07;
        font-family: PlayFair, serif;
        font-size: 2.5rem;
        line-height: 150%;
        margin-right: 2.5rem;
        @media screen and (max-width: 768px) and (min-width: 415px){
          font-size: 1.875rem;
        }
        @media screen and (max-width: 440px) {
          font-size: 1.25rem;
          margin-bottom: 1.875rem!important;
        }
      }
    }
    .main-banner-text {
      width: 32%;
      @media screen and (max-width: 440px) {
        width: 100%;
      }
      .bold-text {
        font-weight: 600;
        color: #2F1D07;
      }
      p {
        color: #2F1D07;
        font-family: Jost, serif;
        font-size: 1rem;
        line-height: 150%;
        margin-bottom: 1rem;
        &:nth-child(2) {
          margin-bottom: 1.875rem;
        }
      }
      button {
        background-color: #E1CAAF;
        color: #2F1D07;
        padding: 1.25rem 1.875rem;
        font-size: 1rem;
        font-family: Jost, serif;
        font-weight: 600;
        line-height: 150%;
        border: none;
        &:hover {
          background-color: #2F1D07;
          color: #FFF8EF;
          transition: .3s;
        }
      }
    }
  }
}
.process-container {
  padding: 0 22.5rem;
  @media screen and (max-width: 1441px) and (min-width: 1300px) {
    padding: 0 11.25rem;
  }
  @media screen and (max-width: 1100px) and (min-width: 769px) {
    padding: 0;
  }
  @media screen and (max-width: 768px) and (min-width: 441px){
    padding: 0;
  }
  @media screen and (max-width: 440px){
    padding: 0;
  }
  h2 {
    color: #2F1D07;
    font-family: PlayFair, serif;
    font-size: 2.5rem;
    line-height: 150%;
    margin-bottom: 6.25rem;
    @media screen and (max-width: 1100px) and (min-width: 769px) {
      padding-left: 1.875rem;
    }
    @media screen and (max-width: 768px) and (min-width: 441px){
      padding-left: 1.25rem;
    }
    @media screen and (max-width: 440px){
      margin-bottom: 3.125rem;
      font-size: 1.25rem;
      padding: 0 1rem;
    }
  }
  .list-group-item {
    border: 1px solid #E1CAAF;
    border-radius: 0;
    width: 100%;
    height: 100%;
    max-width: 24.875rem;
    min-height: 7.375rem;
    flex: 0 0 33.333333%;
    background-color: transparent;
    span {
      color: #E1CAAF;
      font-size: 1rem;
      font-family: Jost, serif;
      line-height: 150%;
      margin-right: 1rem;
    }
    p {
      color: #2F1D07;
      font-family: Jost, serif;
      font-size: 1rem;
      line-height: 150%;
      width: 75%;
    }
    .bold-text {
      color: #2F1D07;
      font-weight: 600;
      width: 100%;
    }
  }
  .list-group-container {
    @media screen and (max-width: 1100px) and (min-width: 769px) {
      justify-content: space-between;
      padding: 0 1.875rem;
    }
    @media screen and (max-width: 768px) and (min-width: 441px){
      justify-content: space-between;
      padding: 0 1.25rem;
    }
    @media screen and (max-width: 440px){
      padding: 0 1rem;
      flex-direction: column;
    }
    .list-group-item {
      @media screen and (max-width: 440px){
        border: 0;
        padding-left: 0!important;
        border-bottom: 1px solid #E1CAAF!important;
        min-height: 7.375rem;
        padding-top: 1.875rem!important;
        padding-bottom: 1.25rem!important;
        &:last-child {
          border: 0!important;
          padding-left: 0!important;
          padding-top: 2rem!important;
        }
      }
      @media screen and (max-width: 768px) and (min-width: 441px){
        max-width: 50%;
        min-height: 7.375rem;
        flex: 0 0 100%;
        &:nth-child(2) {
          border-top: 0;
          border-right: 0;
          padding-left: 2.5rem;
        }
        &:nth-child(3) {
          border: 0;
        }
        &:nth-child(4) {
          border-left: 1px solid #E1CAAF!important;
        }
        &:nth-child(5) {
          border-top: 1px solid #E1CAAF!important;
          border-right: 0;
          border-left: 0;
        }
        &:last-child {
          border-top: 1px solid #E1CAAF!important;
          border-left: 1px solid #E1CAAF!important;
        }
      }
      @media screen and (max-width: 1100px) and (min-width: 769px) {
        max-width: 50%;
        min-height: 7.375rem;
        flex: 0 0 100%;
        &:nth-child(2) {
          border-top: 0;
          border-right: 0;
          padding-left: 2.5rem;
        }
        &:nth-child(3) {
          border-top: 0;
          border-left: 0;
        }
        &:nth-child(4) {
          border-left: 1px solid #E1CAAF!important;
          border: 0;
          border-bottom: 1px solid #E1CAAF!important;
          padding-top: 2.5rem;
        }
        &:nth-child(5) {
          border: 0;
          padding-top: 2.5rem;
          padding-left: 2.5rem;
        }
        &:last-child {
          border-left: 1px solid #E1CAAF!important;
          border: 0;
          padding-top: 2rem;
        }
      }
      &:first-child {
        border-top: 0;
        border-left: 0;
        border-right: 0;
      }
      &:nth-child(2) {
        border-top: 0;
        padding-left: 2.5rem;
      }
      &:nth-child(3) {
        border-right: 0;
        border-top: 0;
        border-left: 0;
      }
      &:nth-child(4) {
        border: 0;
        padding-top: 2.5rem;
      }
      &:nth-child(5) {
        border-top: 0;
        border-bottom: 0;
        padding-top: 2.5rem;
        padding-left: 2.5rem;
      }
      &:last-child {
        border: 0;
        padding-top: 2rem;
      }
    }
  }
  .process-video-container {
    video {
      @media screen and (max-width: 440px){
        margin-top: 0.5rem!important;
        height: 13.125rem;
        margin-bottom: 1.25rem;
      }
      margin: 5rem 0 2.5rem 0;
      height: 31.5rem;
      width: 100%;
      position: relative;
    }
  }
  .process-video-desc {
    @media screen and (max-width: 1100px) and (min-width: 769px) {
      margin-left: 1.875rem;
    }
    @media screen and (max-width: 768px) and (min-width: 441px){
      padding-left: 1.25rem;
    }
    @media screen and (max-width: 440px){
      padding: 0 1rem;
    }
    p {
      color: #2F1D07;
      font-size: 1rem;
      font-family: Jost, serif;
      line-height: 150%;
      &:first-child {
        margin-bottom: 1rem;
      }
    }
  }
}
</style>
