<template>
  <div class="adventages">
    <div class="container">
      <div class="adventages__blocks">
        <div class="adventages__block">
        <img class="adventages__block-img" src="@/assets/img/adventage-1.svg">
        <div class="adventages__block-content">
          <h3 class="adventages__block-title">Команда профессионалов, закрытое Python-комьюнити</h3>
          <p class="adventages__block-text">
            У нас закрытое Python-коммьюнити, в которое входят почти 50 опытных разработчиков. Все специалисты прошли тщательный отбор, обладают подтвержденной квалификацией и высоким уровнем "soft skill".
          </p>
          <a class="adventages__block-link" href="#">Подробнее о том, как мы подбираем кандидатов</a>
        </div>
        </div>
        <div class="adventages__block">
          <div class="adventages__block-content">
            <h3 class="adventages__block-title adventages__block-title--small">Разработка с упором на производство</h3>
            <p class="adventages__block-text">
              Прежде всего мы инженеры, и наше основное предназначение — находить максимально эффективные и экономичные решения бизнес-задачам. В своей работе мы применяем множество разноообразных инструментов и технологий. Неизменным остается только одно - наш стэк: Python, Django, VueJS и ReactJS.
            </p>
          </div>
          <img class="adventages__block-img" src="@/assets/img/adventage-2.svg">
        </div>
        <div class="adventages__block">
          <img class="adventages__block-img" src="@/assets/img/adventage-3.svg">
          <div class="adventages__block-content">
            <h3 class="adventages__block-title adventages__block-title--small">Быстрый старт, минимум бюрократии</h3>
            <p class="adventages__block-text">
              Готовы начать работу в течение одной или двух недель. Для небольших проектов обеспечим минимальную бюрократию - никаких испорченных телефонов, в команде только Вы и исполнитель. Для проектов крупнее - привлечем менеджера и тестировщика.
            </p>
          </div>
        </div>
        <div class="adventages__block">
          <div class="adventages__block-content">
            <h3 class="adventages__block-title">Процессы отработаны, знаем что делаем</h3>
            <p class="adventages__block-text">
              Не усложняем рабочие процессы без явной необходимости. Бережно относимся к ресурсам. Ведем разработку по спринтам или канбану. Автоматизируем процессы деплоя и тестирования. Наши бэкенд-разработчики не боятся фронтенда, а фронтенд-разработчики - бэкенда.
            </p>
          </div>
          <img class="adventages__block-img" src="@/assets/img/adventage-4.svg">
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.adventages {
  padding-top: 101px;
  padding-bottom: 165px;
  &__block:first-child{
    padding-bottom: 104px;
  }
  &__block:not(:first-child):not(:last-child) {
    padding-bottom: 134px;
  }
  &__block {
    display: grid;
    grid-template: 1fr / 1fr 1fr;
    &-img {
      justify-self: center;
      align-self: center;
    }
    &-content {
      align-self: center;
      max-width: 550px;
    }
    &-title {
      font-weight: 800;
      font-size: 36px;
      line-height: 44px;
      padding-bottom: 42px;
      min-width: 585px;
    }
    &-title--small {
      min-width: auto;
      max-width: 475px;
    }
    &-text {
      font-weight: 500;
      font-size: 18px;
      line-height: 28px;
    }
    &-link {
      display: inline-block;
      padding-top: 16px;
      font-weight: 500;
      font-size: 18px;
      line-height: 28px;
      color: $main-color;
      transition: all ease .2s;
    }
    &-link:hover {
      opacity: .5;
    }
  }
}
</style>