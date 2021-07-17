<template>
  <div class="banner-container">
    <div class="main-banner-container d-flex align-items-center justify-content-between">
      <div class="main-banner-title">
        <h2 class="mb-0">Безопастная упаковка для доставки предотвратит появление дефектов.</h2>
      </div>
      <div class="main-banner-text">
        <p class="bold-text">Мы используем для упоковки</p>
        <p>Картонные уголки, гофрокартон, скотч, стретч-пленка, лист двп, воздушно пузырьковую пленку.</p>
        <p class="bold-text mb-0">Можете не переживать о повреждении в дороге. Если пришло с дефектами переделаем бесплатно.</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
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
</style>
