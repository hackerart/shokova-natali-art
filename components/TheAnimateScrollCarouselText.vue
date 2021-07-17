<template>
  <div class="scroll-carousel-container">
    <div class="scroll-carousel-desc-container d-flex flex-column align-items-center">
      <h1>Уникальный декор ручной работы.</h1>
      <p>У каждого художника своя манера и техника исполнения. Поэтому даже при всем желании невозможно создать двух идентичных картин. Каждая работа студии уникальна.</p>
    </div>
    <div class="slider">
      <div class="cursor"></div>
      <div class="slider__wrapper" :style="`left: ${padding}px`">
        <div class="slider__block slider__block_left">
          <img class="slider__img slider__block_margin" src="../static/img/theScrollText/1.png" alt="" />

          <div class="slider__img-block slider__block_margin">
            <img class="slider__img" src="../static/img/theScrollText/2.png" alt="" />
            <img class="slider__img" src="../static/img/theScrollText/3.png" alt="" />
          </div>
        </div>

        <div class="slider__block slider__block_middle">
          <img class="slider__img slider__block_margin" src="../static/img/theScrollText/4.png" alt="" />

          <div class="slider__img-block slider__block_margin">
            <img class="slider__img" src="../static/img/theScrollText/5.png" alt="" />
            <img class="slider__img" src="../static/img/theScrollText/6.png" alt="" />
          </div>

          <img class="slider__img slider__block_margin" src="../static/img/theScrollText/7.png" alt="" />

          <div class="slider__img-block slider__block_margin">
            <img class="slider__img" src="../static/img/theScrollText/2.png" alt="" />
            <img class="slider__img" src="../static/img/theScrollText/3.png" alt="" />
          </div>

          <img class="slider__img slider__block_margin" src="../static/img/theScrollText/4.png" alt="" />
        </div>

        <div class="slider__block slider__block_right">
          <img class="slider__img slider__block_margin" src="../static/img/theScrollText/7.png" alt="" />

          <div class="slider__img-block slider_margin">
            <img class="slider__img" src="../static/img/theScrollText/5.png" alt="" />
            <img class="slider__img" src="../static/img/theScrollText/6.png" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    padding: 0
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
      this.padding = (window.pageYOffset - 2984) * 0.5
    }
  }
}
</script>

<style lang="scss" scoped>
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
</style>
