<template>
  <div class="footer-container">
    <div class="d-flex align-items-start justify-content-between footer-main-mob-container">
      <div class="footer-logo-container">
        <img src="../static/img/footer/logo.png" alt="">
      </div>
      <div class="footer-link-container d-flex align-items-center">
        <a href="#process">Процесс</a>
        <a href="#">Услуги</a>
        <a href="#">Картины</a>
        <a href="#">Столы</a>
        <a href="#">Часы</a>
      </div>
      <div class="footer-contact-container d-flex flex-column">
        <a href="tel:+74958632812">7 (495) 863-28-12</a>
        <a href="mailto:info@shokonanatali">info@shokonanatali</a>
      </div>
    </div>
    <div class="d-flex align-items-end justify-content-between footer-law-container">
      <div class="d-flex align-items-center footer-mob-text-law-container">
        <p class="mb-0">2021-2025 ©Все права защищены</p>
        <a href="#">Политика конфиденциальности</a>
      </div>
      <a href="#top"><button><img src="../static/img/footer/arrow.png" alt=""></button></a>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.footer-container {
  padding: 1.375rem 22.5rem 3.125rem 22.5rem;
  @media screen and (max-width: 1100px) and (min-width: 999px){
    padding: 1.375rem 1.875rem 3.125rem 1.875rem;
  }
  @media screen and (max-width: 999px) and (min-width: 415px){
    padding: 1.375rem 1.25rem 3.125rem 1.25rem;
  }
  @media screen and (max-width: 440px){
    padding: 6.25rem 0 3.125rem;
    .footer-main-mob-container {
      flex-direction: column;
      .footer-logo-container {
        width: 100%;
        justify-content: center;
        display: flex;
        margin-bottom: 2.25rem;
      }
      .footer-link-container {
        flex-direction: column;
        align-items: center;
        width: 100%;
        padding-bottom: 2.25rem;
        a {
          margin-right: 0;
          margin-bottom: 1.25rem;
          &:last-child {
            margin-bottom: 0;
          }
        }
      }
      .footer-contact-container {
        width: 100%;
        align-items: center;
      }
    }
    .footer-law-container {
      flex-direction: column-reverse;
      align-items: center!important;
      button {
        margin-bottom: 2.25rem;
      }
      .footer-mob-text-law-container {
        flex-direction: column;
        width: 100%;
        p {
          margin-right: 0;
          margin-bottom: 1.875rem;
        }
      }
    }
  }
  .footer-link-container {
    a {
      color: #2F1D07;
      font-family: Jost, serif;
      font-size: 1rem;
      line-height: 150%;
      margin-right: 2.25rem;

      &:last-child {
        margin-right: 0;
      }
    }
  }
  .footer-contact-container {
    a {
      color: #2F1D07;
      font-family: Jost, serif;
      font-size: 1rem;
      line-height: 150%;
      &:first-child {
        margin-bottom: 1rem;
      }
    }
  }
  .footer-law-container {
    padding-top: 2.875rem;
    p {
      color: #2F1D07;
      font-family: Jost, serif;
      font-size: .875rem;
      line-height: 1.25rem;
      letter-spacing: 0.02em;
      margin-right: 12.25rem;
    }
    a {
      color: #2F1D07;
      font-family: Jost, serif;
      font-size: .875rem;
      line-height: 1.25rem;
      letter-spacing: 0.02em;
      text-decoration: underline;
    }
    button {
      background-color: #E1CAAF;
      border: 0;
      padding: .875rem 1.125rem;
    }
  }
}
</style>
