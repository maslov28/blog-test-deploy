<template>
  <section class="feedback">
    <div class="container">
      <h2 class="feedback__title">Отзывы</h2>
      <div class="feedback__content">
        <div class="feedback__content-left">
          <h4 class="feedback__source">Upwork 100% Job success</h4>
          <span class="feedback__count">8 отзывов</span>
        </div>
        <div class="feedback__content-right">
          <div class="feedback__slider">
            <div class="feedback__slider-wrapper">
              <carousel-slider 
                :prevNextBtn="true"
                :countSlide="3"
              >
                <div class="feedback__slider-item">
                  <p class="feedback__slider-text">
                    Dmitry and his team are excellent python/django developers, and I would recommend them to anyone who needs this type of ...
                  </p>
                  <div class="feedback__slider-item-autor">
                    <span class="feedback__slider-autor-name">Simon J.</span>
                    <p class="feedback__slider-autor-position">
                      Project Manager at <a class="highlight" href="#">Company.io</a>
                    </p>
                  </div>
                  <a class="feedback__slider-show-original highlight" href="#">Оригинал отзыва</a>
                </div>
                <div class="feedback__slider-item">
                  <p class="feedback__slider-text">
                    Dmitry and his team are excellent python/django developers, and I would recommend them to anyone who needs this type of ...
                  </p>
                  <div class="feedback__slider-item-autor">
                    <span class="feedback__slider-autor-name">Simon J.</span>
                    <p class="feedback__slider-autor-position">
                      Project Manager at <a class="highlight" href="#">Company.io</a>
                    </p>
                  </div>
                  <a class="feedback__slider-show-original highlight" href="#">Оригинал отзыва</a>
                </div>
                <div class="feedback__slider-item">
                  <p class="feedback__slider-text">
                    Dmitry and his team are excellent python/django developers, and I would recommend them to anyone who needs this type of ...
                  </p>
                  <div class="feedback__slider-item-autor">
                    <span class="feedback__slider-autor-name">Simon J.</span>
                    <p class="feedback__slider-autor-position">
                      Project Manager at <a class="highlight" href="#">Company.io</a>
                    </p>
                  </div>
                  <a class="feedback__slider-show-original highlight" href="#">Оригинал отзыва</a>
                </div>
              </carousel-slider>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import CarouselSlider from "@/components/common/slider/carousel-slider.vue";

export default {
  components: {
    CarouselSlider
  }
}
</script>

<style  lang="scss">
.feedback {
  background-color: $section-bg-dark;
  padding-top: 96px;
  padding-bottom: 181px;
  &__title {
    font-weight: 800;
    font-size: 48px;
    line-height: 59px;
    text-align: center;
    padding-bottom: 80px;
  }
  &__content {
    display: flex;
    justify-content: space-between;
    position: relative;
    &-right {
      position: absolute;
      top: 0;
      right: -100px;
    }
  }
  &__source {
    position: relative;
    font-weight: 800;
    font-size: 20px;
    line-height: 28px;
    max-width: 268px;
    padding-bottom: 19px;
    padding-left: 89px;
  }
  &__source::before {
    content: '';
    position: absolute;
    background: url('@/assets/img/crown-icon-blue.svg') no-repeat center center;
    top: 2px;
    left: 0;
    min-width: 50px;
    min-height: 58px;
  }
  &__count {
    padding-left: 89px;
    font-weight: 500;
    font-size: 18px;
    line-height: 28px;
  }
}
.feedback__slider {
  position: relative;
  &-wrapper {
    min-width: 760px;
    display: flex;
    justify-content: center;
  }
  &-item {
      position: relative;
      min-width: 560px;
    }
    &-text {
      max-width: 560px;
      font-weight: 500;
      font-size: 18px;
      line-height: 28px;
      padding-bottom: 39px;
    }
    &-autor-name {
      position: relative;
      font-weight: 600;
      font-size: 16px;
      line-height: 20px;
      padding-bottom: 6px;
      padding-right: 30px;
    }
    &-autor-name::after {
      content: '';
      position: absolute;
      top: 0;
      right: 0;
      width: 18px;
      height: 18px;
      background: url('@/assets/img/facebook-logo-dark.svg') no-repeat center center;
    }
    &-autor-position {
      font-size: 14px;
      line-height: 24px;
      color: $text-color-blur;
    }
    &-show-original {
      position: absolute;
      bottom: 0;
      right: 0;
      font-size: 14px;
      line-height: 24px;
    }
}
.slider__prev-btn-wrapper {
  position: absolute;
  top: 70px;
  left: 0;
}
.slider__next-btn-wrapper {
  position: absolute;
  top: 70px;
  right: 0;
}
.slider__items {
  max-width: 560px;
}
.highlight {
  transition: all ease .2s;
}
.highlight:hover {
  opacity: .5;
}
</style>