<template>
  <div class="header__top">
      <img class="header__top-logo" src="@/assets/img/logo-white.svg" alt="logo">
      <header-navigate></header-navigate>
      <div class="header__links-block">
        <a class="header__top-phone" href="tel: +74994344344">+7 (499) 434-43-44</a>
        <a class="header__top-language" href="#">En</a>
      </div>
  </div>
</template>

<script>
import HeaderNavigate from './navigate/HeaderNavigate.vue'
export default {
  components: {HeaderNavigate}
}
</script>

<style lang="scss">
  .header__top {
    display: flex;
    align-items: center;
    padding: 31px 40px 31px 40px;
    justify-content: space-between;
    font-weight: 600;
    &-phone {
      margin-right: 70px;
      transition: all ease .2s;
    }
    &-phone:hover {
      opacity: .5;
    }
    &-language {
      transition: all ease .2s;
    }
    &-language:hover {
      opacity: .5;
    }
  }
</style>