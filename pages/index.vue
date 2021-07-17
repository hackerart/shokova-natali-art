<template>
  <div class="app">
    <div class="background-line">
      <Navbar />
      <TheMainHeadline />
    </div>
    <div class="background-line-reverse">
      <TheProcessVideo />
      <TheHeadline />
    </div>
    <TheBanner />
    <TheAnimateScrollCarouselText />
    <TheDeliveryBanner />
    <TheCarousel />
    <TheAnimateScrollCarousel />
    <TheConsult />
    <Footer />
  </div>
</template>

<script>
import TheMainHeadline from "../components/TheMainHeadline";
import TheConsult from "../components/TheConsult";
import TheProcessVideo from "../components/TheProcessVideo";
import TheHeadline from "../components/TheHeadline";
import TheBanner from "../components/TheBanner";
import TheDeliveryBanner from "../components/TheDeliveryBanner";
import TheCarousel from "../components/TheCarousel";
import Footer from "../components/Footer";
import TheAnimateScrollCarousel from "../components/TheAnimateScrollCarousel";
import TheAnimateScrollCarouselText from "../components/TheAnimateScrollCarouselText";

export default {
  components: {
    TheAnimateScrollCarouselText,
    TheAnimateScrollCarousel,
    Footer,
    TheCarousel,
    TheDeliveryBanner,
    TheBanner,
    TheHeadline,
    TheProcessVideo,
    TheConsult,
    TheMainHeadline,
  }
}
</script>

<style lang="scss">
html {
  scroll-behavior: smooth;
}
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Jost&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Jost:wght@600&disp lay=swap');
.app {
  background-color: #FFF8EF;
  .background-line {
    background-image: url("../static/img/theMainHeadline/back.png");
    background-repeat: no-repeat;
    background-position: right;
    @media screen and (max-width: 1100px) {
      background-image: none;
    }
  }
  .background-line-reverse {
    background-image: url("../static/img/theHeadline/back.png");
    background-repeat: no-repeat;
    background-position: left bottom 0%;
    @media screen and (max-width: 1100px) {
      background-image: none;
    }
  }
}

</style>


