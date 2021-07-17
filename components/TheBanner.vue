<template>
  <div class="banner-container">
    <div class="main-banner-container d-flex align-items-center justify-content-between">
      <div class="main-banner-title">
        <h2 class="mb-0">Наши дизайнеры бесплатно помогут подобрать декор для вашего интерьера.</h2>
      </div>
      <div class="main-banner-text">
        <p>Вы в вайбере или телеграмме отправяете фотографию вашего интерьера, где будет размещаться картина, часы или стол.</p>
        <button>
          Записаться на консультацию
        </button>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.banner-container {
  padding: 12.5rem 11.25rem;
  background-image: url("../static/img/theBanner/back.png");
  background-repeat: no-repeat;
  background-position: right 2% bottom;
  @media screen and (max-width: 1441px) and (min-width: 1300px) {
    background-position: right 3% bottom;
  }
  @media screen and (max-width: 1100px) and (min-width: 415px){
    background-image: none;
    padding: 9.375rem 0;
  }
  @media screen and (max-width: 415px) {
    background-image: none;
    padding: 6.25rem 0 0 0;
  }
  .main-banner-container {
    padding: 6.25rem 11.25rem;
    background-color: #F3E6D7;
    @media screen and (max-width: 1441px) and (min-width: 1300px) {
      padding: 6.25rem 3.25rem;
    }
    @media screen and (max-width: 1100px) and (min-width: 769px){
      padding: 6.25rem 1.875rem;
      align-items: flex-start!important;
    }
    @media screen and (max-width: 768px) and (min-width: 415px){
      padding: 3.125rem 1.875rem;
    }
    @media screen and (max-width: 440px) {
      flex-direction: column;
      padding: 3.125rem 1rem;
    }
    .main-banner-title {
      width: 45%;
      @media screen and (max-width: 1100px) and (min-width: 769px){
        width: 60%;
      }
      @media screen and (max-width: 1441px) and (min-width: 1300px) {
        width: 55%;
      }
      @media screen and (max-width: 768px) and (min-width: 441px){
        width: 50%;
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
        }
        @media screen and (max-width: 440px) {
          margin-bottom: 1.875rem!important;
        }
      }
    }
    .main-banner-text {
      width: 33%;
      @media screen and (max-width: 1100px) and (min-width: 415px){
        width: 42%;
      }
      @media screen and (max-width: 440px) {
        width: 100%;
      }
      p {
        color: #2F1D07;
        font-family: Jost, serif;
        font-size: 1rem;
        line-height: 150%;
        margin-bottom: 1.875rem;
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
        @media screen and (max-width: 440px) {
          width: 100%;
        }
      }
    }
  }
}
</style>
