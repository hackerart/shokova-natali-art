<template>
  <div class="consult-container d-flex align-items-center justify-content-center">
    <div class="main-consult-container d-flex align-items-center">
      <div class="main-consult-title-container">
        <h2>Получить бесплатную консультацию.</h2>
        <p>Выберите удобный для вас мессенджер. И давайте приступим к улучшению вашего интерьера.</p>
      </div>
      <div class="main-consult-form-container">
        <p>Способ связи</p>
        <b-form-select v-model="selected" :options="options"></b-form-select>
        <button>Записаться на консультацию</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      selected: 'a',
      options: [
        { value: 'a', text: 'Telegram' },
        { value: 'b', text: 'Whatsapp' },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.consult-container {
  background-image: url("../static/img/theBanner/back.png");
  background-repeat: no-repeat;
  background-position: right 2% bottom;
  padding: 12.5rem 11.25rem;
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

  .main-consult-container {
    background-color: #F3E6D7;
    padding: 6.25rem 11.25rem;
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
    .main-consult-title-container {
      h2 {
        font-family: PlayFair, serif;
        font-size: 2.5rem;
        line-height: 150%;
        color: #2F1D07;
        margin-bottom: 1.875rem;
        width: 70%;
        @media screen and (max-width: 1441px) and (min-width: 1300px) {
          width: 80%;
        }
        @media screen and (max-width: 1100px) and (min-width: 415px){
          width: 80%;
        }
        @media screen and (max-width: 768px) and (min-width: 415px){
          font-size: 1.875rem;
        }
        @media screen and (max-width: 440px) {
          font-size: 1.25rem;
        }
      }
      p {
        font-family: Jost, serif;
        font-size: 1rem;
        line-height: 150%;
        color: #2F1D07;
        margin-bottom: 0;
        width: 60%;
        @media screen and (max-width: 1441px) and (min-width: 1300px) {
          width: 80%;
        }
        @media screen and (max-width: 1100px) and (min-width: 415px){
          width: 80%;
        }
        @media screen and (max-width: 440px) {
          padding-bottom: 1.875rem;
          width: 100%;
        }
      }
    }
    .main-consult-form-container {
      p {
        font-family: Jost, serif;
        font-weight: 600;
        font-size: 1rem;
        line-height: 150%;
        color: #2F1D07;
        margin-bottom: 1.25rem;
      }
      .custom-select {
        background-color: transparent;
        border: 1px solid #2F1D07;
        box-sizing: border-box;
        border-radius: 0;
        padding: 20px 25px;
        min-width: 290px;
        width: 100%;
        max-width: 560px;
        height: 100%;
        background: url(./static/img/theConsult/arrow.png) right 0.75rem center/10px 5px no-repeat;
        margin-bottom: 1.875rem;
        font-family: Jost, serif;
        font-size: 1rem;
        line-height: 150%;
        color: #2F1D07;
        &:focus {
          box-shadow: none;
        }
      }
      button {
        background-color: #E1CAAF;
        border: none;
        color: #2F1D07;
        font-family: Jost, serif;
        font-weight: 600;
        font-size: 1rem;
        padding: 1.25rem 1.875rem;
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
