<template>
  <div class="headline-container container-fluid px-0">
    <div class="position-absolute headline-backgroundImg">
      <div class="headline-backgroundImg-img-1">
        <img src="../static/img/theHeadline/1.png" alt="">
      </div>
      <div class="headline-backgroundImg-img-2">
        <img src="../static/img/theHeadline/2.png" alt="">
      </div>
    </div>
    <div class="position-absolute headline-backgroundImg background-position-right">
      <div class="headline-backgroundImg-img-1-reverse">
        <img src="../static/img/theHeadline/3.png" alt="">
      </div>
      <div class="headline-backgroundImg-img-2-reverse">
        <img src="../static/img/theHeadline/4.png" al t="">
      </div>
    </div>
    <div class="headline-title d-flex flex-column align-items-center">
      <h1>Мы всегда кропотливо подбираем то, <br> что понравится заказчику и придаст индивидуальность интерьеру.</h1>
    </div>
  </div>
</template>

<script>

</script>

<style lang="scss" scoped>
.headline-container {
  padding-top: 12.5rem;
  padding-bottom: .8rem;

  .background-position-right {
    right: 0;
    display: flex;
    flex-direction: column;
    align-items: flex-end;
  }
  .headline-backgroundImg {
    .headline-backgroundImg-img {
      &-1 {
        margin-bottom: 5rem;
      }
      &-2 {
        margin-left: 22.5rem;
      }
      &-1-reverse {
        margin-bottom: 5rem;
        margin-right: 22.5rem;
      }
      @media screen and (max-width: 1441px) and (min-width: 1300px) {
        &-1 {
          margin-bottom: 8rem;
        }
        &-2 {
          margin-left: 15.5rem;
        }
        &-1-reverse {
          margin-bottom: 8rem;
          margin-right: 10.5rem;
        }
      }
      @media screen and (max-width: 1100px) and (min-width: 769px){
        &-1 {
          display: none;
        }
        &-2 {
          margin-left: 0;
          margin-top: 260%;
        }
        &-1-reverse {
          margin-right: 0;
        }
        &-2-reverse {
          display: none;
        }
      }
      @media screen and (max-width: 768px) and (min-width: 441px){
        &-1 {
          display: none;
        }
        &-2 {
          margin-left: 0;
          margin-top: 260%;
        }
        &-1-reverse {
          margin-right: 0;
        }
        &-2-reverse {
          display: none;
        }
      }
      @media screen and (max-width: 440px){
        &-1 {
          display: none;
        }
        &-2 {
          margin-left: 0;
          margin-top: 260%;
          img {
            width: 5.3125rem;
            height: 6.25rem;
          }
        }
        &-1-reverse {
          margin-right: 0;
          img {
            width: 5.3125rem;
            height: 6.25rem;
          }
        }
        &-2-reverse {
          display: none;
        }
      }
    }
  }
  .headline-title {
    h1 {
      font-size: 3.75rem;
      font-family: Playfair Display,serif;
      line-height: 150%;
      text-transform: uppercase;
      color: #2F1D07;
      width: 45%;
      text-align: center;
      margin-bottom: 1.875rem;
      @media screen and (max-width: 1441px) and (min-width: 1300px) {
        width: 60%;
      }
      @media screen and (max-width: 1100px) and (min-width: 769px){
        width: 77%;
        z-index: 2;
      }
      @media screen and (max-width: 768px) and (min-width: 441px){
        width: 84%;
        font-size: 3.125rem;
        z-index: 2;
      }
      @media screen and (max-width: 440px){
        z-index: 2;
        font-size: 1.5625rem;
        width: 70%;
      }
    }
  }
}
</style>
