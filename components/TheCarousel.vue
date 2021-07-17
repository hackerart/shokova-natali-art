<template>
  <div class="carousel-container">
    <div class="d-flex justify-content-center">
      <h1>Декор, который мы делаем.</h1>
    </div>
    <client-only>
      <carousel v-bind="options" class="carousel-main-container">
        <slide class="img-wrapper">
          <img src="../static/img/theCarousel/1.png" />
        </slide>
        <slide class="img-wrapper">
          <img src="../static/img/theCarousel/2.png" />
        </slide>
        <slide class="img-wrapper">
          <img src="../static/img/theCarousel/3.png" />
        </slide>
      </carousel>
    </client-only>
  </div>
</template>

<script>
export default {
  data() {
    return {
      options: {
        autoplay: true,
        paginationEnabled: false,
        scrollPerPage: false,
        perPage: 3,
      },
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
    h1 {
      color: #2F1D07;
      font-family: PlayFair, serif;
      font-size: 3.75rem;
      line-height: 150%;
      text-transform: uppercase;
      margin-bottom: 6.25rem;
      width: 50%;
      text-align: center;
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
</style>
