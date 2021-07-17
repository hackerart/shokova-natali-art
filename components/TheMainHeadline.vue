<template>
  <div class="mainHeadline-container container-fluid px-0">
    <div class="position-absolute mainHeadline-backgroundImg">
      <div class="mainHeadline-backgroundImg-img-1">
        <img src="../static/img/theMainHeadline/1.png" alt="">
      </div>
      <div class="mainHeadline-backgroundImg-img-2">
        <img src="../static/img/theMainHeadline/2.png" alt="">
      </div>
    </div>
    <div class="position-absolute mainHeadline-backgroundImg background-position-right">
      <div class="mainHeadline-backgroundImg-img-1-reverse">
        <img src="../static/img/theMainHeadline/3.png" alt="">
      </div>
      <div class="mainHeadline-backgroundImg-img-2-reverse">
        <img src="../static/img/theMainHeadline/4.png" alt="">
      </div>
    </div>
    <div class="mainHeadline-title d-flex flex-column align-items-center">
      <h1>Создание картин, часов и других предметов декора на заказ.</h1>
      <p>Мы занимаемся написанием интерьерных картин в современных техниках
        и созданием часов и других элементов декора.</p>
      <button>
        Записаться на консультацию
      </button>
    </div>
  </div>
</template>

<script>

</script>

<style lang="scss" scoped>
.mainHeadline-container {
  padding: 7.5rem 0 10.6rem;
  margin-bottom: 9.4rem;
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
  .mainHeadline-backgroundImg {
    .mainHeadline-backgroundImg-img {
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
      &-2-reverse {
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
      width: 18.5%;
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
</style>
