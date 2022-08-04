<template>
  <section class="projects">
    <div class="container">
      <h2 class="projects__title">Проекты</h2>
      <p class="projects__subtitle">
        Мы опубликовываем только малую часть наших работ, так как большинство
        проектов находятся под NDA
      </p>
      <div class="projects__slider">
        <carousel-slider :dotBtn="true" :countSlide="4">
          <div class="slider__item">
            <a class="slider__item-block slider__item-block--a" href="#">
              <img class="slider__item-bg" src="@/assets/img/boat-bg.jpg" />
              <div class="slider__item-content">
                <h4 class="slider__item-title">SailSpeak</h4>
                <p class="slider__item-text">
                  Разработка маркетплейса по аренде яхт SailSpeak
                </p>
              </div>
            </a>
            <a class="slider__item-block slider__item-block--b" href="#">
              <img class="slider__item-bg" src="@/assets/img/car-bg.jpg" />
              <div class="slider__item-content">
                <h4 class="slider__item-title">Быстрые займы</h4>
                <p class="slider__item-text">
                  Разработка промо-сайта займы под залог ПТС
                </p>
              </div>
            </a>
            <a class="slider__item-block slider__item-block--c" href="#">
              <img
                class="slider__item-bg"
                src="@/assets/img/sculpture-bg.jpg"
              />
              <div class="slider__item-content">
                <h4 class="slider__item-title">iReg</h4>
                <p class="slider__item-text">
                  Система регистрирует авторское право по цене чашки кофе
                </p>
              </div>
            </a>
          </div>
          <div class="slider__item">
            <a class="slider__item-block slider__item-block--a" href="#">
              <img class="slider__item-bg" src="@/assets/img/boat-bg.jpg" />
              <div class="slider__item-content">
                <h4 class="slider__item-title">SailSpeak</h4>
                <p class="slider__item-text">
                  Разработка маркетплейса по аренде яхт SailSpeak
                </p>
              </div>
            </a>
            <a class="slider__item-block slider__item-block--b" href="#">
              <img class="slider__item-bg" src="@/assets/img/car-bg.jpg" />
              <div class="slider__item-content">
                <h4 class="slider__item-title">Быстрые займы</h4>
                <p class="slider__item-text">
                  Разработка промо-сайта займы под залог ПТС
                </p>
              </div>
            </a>
            <a class="slider__item-block slider__item-block--c" href="#">
              <img
                class="slider__item-bg"
                src="@/assets/img/sculpture-bg.jpg"
              />
              <div class="slider__item-content">
                <h4 class="slider__item-title">iReg</h4>
                <p class="slider__item-text">
                  Система регистрирует авторское право по цене чашки кофе
                </p>
              </div>
            </a>
          </div>
          <div class="slider__item">
            <a class="slider__item-block slider__item-block--a" href="#">
              <img class="slider__item-bg" src="@/assets/img/boat-bg.jpg" />
              <div class="slider__item-content">
                <h4 class="slider__item-title">SailSpeak</h4>
                <p class="slider__item-text">
                  Разработка маркетплейса по аренде яхт SailSpeak
                </p>
              </div>
            </a>
            <a class="slider__item-block slider__item-block--b" href="#">
              <img class="slider__item-bg" src="@/assets/img/car-bg.jpg" />
              <div class="slider__item-content">
                <h4 class="slider__item-title">Быстрые займы</h4>
                <p class="slider__item-text">
                  Разработка промо-сайта займы под залог ПТС
                </p>
              </div>
            </a>
            <a class="slider__item-block slider__item-block--c" href="#">
              <img
                class="slider__item-bg"
                src="@/assets/img/sculpture-bg.jpg"
              />
              <div class="slider__item-content">
                <h4 class="slider__item-title">iReg</h4>
                <p class="slider__item-text">
                  Система регистрирует авторское право по цене чашки кофе
                </p>
              </div>
            </a>
          </div>
          <div class="slider__item">
            <a class="slider__item-block slider__item-block--a" href="#">
              <img class="slider__item-bg" src="@/assets/img/boat-bg.jpg" />
              <div class="slider__item-content">
                <h4 class="slider__item-title">SailSpeak</h4>
                <p class="slider__item-text">
                  Разработка маркетплейса по аренде яхт SailSpeak
                </p>
              </div>
            </a>
            <a class="slider__item-block slider__item-block--b" href="#">
              <img class="slider__item-bg" src="@/assets/img/car-bg.jpg" />
              <div class="slider__item-content">
                <h4 class="slider__item-title">Быстрые займы</h4>
                <p class="slider__item-text">
                  Разработка промо-сайта займы под залог ПТС
                </p>
              </div>
            </a>
            <a class="slider__item-block slider__item-block--c" href="#">
              <img
                class="slider__item-bg"
                src="@/assets/img/sculpture-bg.jpg"
              />
              <div class="slider__item-content">
                <h4 class="slider__item-title">iReg</h4>
                <p class="slider__item-text">
                  Система регистрирует авторское право по цене чашки кофе
                </p>
              </div>
            </a>
          </div>
        </carousel-slider>
      </div>
    </div>
  </section>
</template>

<script>
import CarouselSlider from "@/components/common/slider/carousel-slider.vue";
export default {
  components: {
    CarouselSlider,
  },
};
</script>

<style lang="scss">
.projects {
  padding-top: 140px;
  padding-bottom: 140px;
  &__title {
    font-weight: 800;
    font-size: 48px;
    line-height: 59px;
    text-align: center;
    padding-bottom: 32px;
  }
  &__subtitle {
    text-align: center;
    max-width: 553px;
    margin: 0 auto;
    padding-bottom: 83px;
  }
}
.slider__item {
  min-width: 1160px;
  display: grid;
  gap: 40px;
  grid-template-areas:
    "a c"
    "b c";
  &-block {
    position: relative;
  }
  &-content {
    position: absolute;
    bottom: 40px;
    left: 40px;
    color: $text-color-light;
  }
  &-title {
    font-weight: 800;
    font-size: 24px;
    line-height: 28px;
    padding-bottom: 16px;
  }
  &-text {
    font-size: 16px;
    line-height: 24px;
  }
  &-block {
    transition: all ease .2s;
  }
  &-block:hover {
    box-shadow: 0px 5px 10px 0px rgba(0, 0, 0, 0.5);
    opacity: .8;
  }
  &-block--a {
    grid-area: a;
  }
  &-block--a .slider__item-text {
    max-width: 240px;
  }
  &-block--b {
    grid-area: b;
  }
  &-block--b .slider__item-text {
    max-width: 240px;
  }
  &-block--c {
    grid-area: c;
  }
  &-block--c .slider__item-text {
    max-width: 325px;
  }
}
</style>