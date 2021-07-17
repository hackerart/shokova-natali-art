<template>
  <div>
    <b-navbar toggleable="sm" type="light" class="p-0 container" id="top">
      <b-collapse id="nav-text-collapse" is-nav class="justify-content-center">
        <b-navbar-nav>
          <a href="#process" class="link-d-none">Процесс</a>
          <a href="#" class="link-d-none">Услуги</a>
          <NuxtLink to="/picture"><a href="#" >Картины</a></NuxtLink>
          <a href="#">Столы</a>
          <a href="#">Часы</a>
        </b-navbar-nav>
      </b-collapse>
      <b-navbar-brand class="mr-0"><img src="../static/img/nav/logo.png" alt="logo"></b-navbar-brand>
      <b-collapse id="nav-text-collapse" is-nav class="justify-content-center align-items-start">
        <b-navbar-nav class="second-navbar-nav">
          <div>
            <div class="d-flex align-items-center">
              <button>Whatsapp</button>
              <button>Telegram</button>
            </div>
            <p>Доставим в любую точки мира</p>
          </div>
        </b-navbar-nav>
      </b-collapse>
      <b-navbar-toggle target="nav-text-collapse"></b-navbar-toggle>
    </b-navbar>
  </div>
</template>

<style lang="scss" scoped>
@media screen and (min-width: 576px) and (max-width: 991px) {
  .link-d-none {
    display: none;
  }
  .second-navbar-nav {
    padding-left: 0 !important;
  }
}

.navbar {
  justify-content: space-between;
}
.navbar-collapse {
  flex-grow: 0;
}
.navbar-brand {
  justify-content: center;
  display: flex;
}
.second-navbar-nav {
  padding-left: 9.375rem;
}
.navbar-nav {
  height: 100%;
  a {
    color: #2F1D07;
    margin-right: 2.25rem;
    font-size: 1rem;
    font-family: Jost, serif;
    &:last-child {
      margin-right: 0;
    }
  }
  button {
    background-color: transparent;
    border: 1px solid #E1CAAF;
    padding: 1.25rem 1.875rem;
    font-size: 1rem;
    line-height: 150%;
    color: #2F1D07;
    font-family: Jost, serif;
    &:hover {
      border-color: #2F1D07;
    }
  }
  p {
    padding-top: 15px ;
    font-size: 1rem;
    line-height: 150%;
    color: #33210C;
    margin-bottom: 0;
    text-align: right;
    font-family: Jost, serif;
  }
}
</style>
