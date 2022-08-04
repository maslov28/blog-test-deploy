<template>
  <header class="header">
    <!-- Шапка -->
    <header-top></header-top>
    <!-- Основной контент хедера -->
    <div class="container">
      <div class="header__main">
        <!-- Левая чать хедера -->
        <div class="header__main-left">
          <h1 class="header__title">Веб-разработчики на Python и Django</h1>
          <p class="header__subtitle">
            Проектируем, разрабытывам и развиваем сложные веб-проекты
          </p>
          <action-button color="main-color">Обсудить проект</action-button>
        </div>
        <!-- Правая чать хедера -->
        <div class="header__main-right">
          <div class="header__benefit">
            <img
              class="header__benefit-icon"
              src="@/assets/img/pedestal-icon.svg"
            />
            <p class="header__benefit-text">7 лет на рынке</p>
          </div>
          <div class="header__benefit">
            <img
              class="header__benefit-icon"
              src="@/assets/img/specialist-icon.svg"
            />
            <p class="header__benefit-text">48 специалиста</p>
          </div>
          <div class="header__benefit">
            <img
              class="header__benefit-icon"
              src="@/assets/img/crown-icon.svg"
            />
            <p class="header__benefit-text">Upwork 100% Job success</p>
          </div>
        </div>
      </div>
      <!-- Нижняя чать хедера -->
      <div class="header__bottom">
        <social-links></social-links>
      </div>
    </div>
  </header>
</template>

<script>
import HeaderTop from "./header/HeaderTop.vue";
import SocialLinks from "@/components/common/social/SocialLinks.vue";
import ActionButton from "@/components/common/buttons/ActionButton.vue"

export default {
  components: { 
    HeaderTop, 
    SocialLinks,
    ActionButton 
  },
};
</script>

<style lang="scss">
.header {
  background: url('@/assets/img/start-bg.jpg');
  background-size: cover;
  padding-bottom: 50px;
  color: $text-color-light;
  a {
    color: inherit;
  }
  &__main {
    display: flex;
    padding-top: 118px;
    padding-bottom: 156px;
  }
  &__main-left {
    max-width: 676px;
  }
  &__main-right {
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding-left: 147px;
  }
  &__title {
    font-weight: 800;
    font-size: 62px;
    line-height: 84px;
    padding-bottom: 21px;
  }
  &__subtitle {
    max-width: 461px;
    font-weight: 500;
    font-size: 18px;
    line-height: 28px;
    padding-bottom: 64px;
  }
  &__benefit:not(:last-child) {
    padding-bottom: 70px;
  }
  &__benefit {
    display: flex;
    align-items: center;
    &-text {
      padding-left: 40px;
    }
  }
}
</style>