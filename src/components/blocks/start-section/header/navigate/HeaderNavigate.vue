<template>
  <nav class="navigate">
    <ul class="navigate__list">
      <li class="navigate__list-item">
        <a class="navigate__list-link navigate__list-link--arrow" href="#">О нас</a>
      </li>
      <li class="navigate__list-item ">
        <a class="navigate__list-link navigate__list-link--arrow" href="#">Услуги</a>
      </li>
      <li class="navigate__list-item">
        <a class="navigate__list-link navigate__list-link--arrow" href="#">Аутсорс</a>
      </li>
      <li class="navigate__list-item">
        <a class="navigate__list-link" href="#">Кейсы</a>
      </li>
      <li class="navigate__list-item">
        <a class="navigate__list-link" href="#">Карьера</a>
      </li>
      <li class="navigate__list-item">
        <a class="navigate__list-link navigate__list-link--arrow" href="#">Блог</a>
      </li>
      <li class="navigate__list-item">
        <a class="navigate__list-link" href="#">Контакты</a>
      </li>
    </ul>
  </nav>
</template>

<style lang="scss">
  .navigate__list {
    display: flex;
    list-style: none;
    &-item:not(:last-child) {
      margin-right: 32px;
    }
    &-link {
      transition: all ease .2s;
    }
    &-link:hover {
      opacity: .5;
    }
    &-link--arrow {
      position: relative;
    }
    &-link--arrow::after {
      content: '';
      position: absolute;
      width: 8px;
      height: 4px;
      top: 0;
      bottom: 0;
      margin: auto;
      margin-left: 6px;
      background: url("@/assets/img/arrow-down.svg") no-repeat center center;
    }
  }

</style>
