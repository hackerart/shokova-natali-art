<template>
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
    <div class="process-video-container">
      <video src="../static/video/video.mp4" controls></video>
    </div>
    <div class="process-video-desc">
      <p>Процесс создания часов из эпоксидной смолы</p>
      <p class="mb-0">Длительность: 5 минут</p>
    </div>
  </div>
</template>

<script>
</script>

<style lang="scss" scoped>
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
