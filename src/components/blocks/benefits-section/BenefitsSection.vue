<template>
  <div class="benefits">
    <div class="container">
      <div class="benefits__cards">
        <div class="benefit__card benefit__card--small">
          <img class="benefit__card-logo" src="@/assets/img/umbrella-ico.svg" alt="umbrella ico">
          <h3 class="benefit__card-title">Экономим ваши время и деньги</h3>
          <p class="benefit__card-text">
            С нами работать выгоднее, чем нанимать специалистов в штат или работать с фрилансерами
          </p>
        </div>
        <div class="benefit__card benefit__card--small">
          <img class="benefit__card-logo" src="@/assets/img/armor-ico.svg" alt="armor ico">
          <h3 class="benefit__card-title">Минимизируем риски</h3>
          <p class="benefit__card-text">
            Предоставляем до 20 бесплатных тестовых часов для знакомства с нами и принятия решения о совместной работе
          </p>
        </div>
        <div class="benefit__card">
          <img class="benefit__card-logo" src="@/assets/img/dartboard-ico.svg" alt="dartboard ico">
          <h3 class="benefit__card-title">Стабильное высокое качество</h3>
          <p class="benefit__card-text">
            Работаем только с узким стеком: Django, React и Vue. Все специалисты обладают высокой подтвержденной квалификацией.
          </p>
        </div>
        <div class="benefit__card">
          <img class="benefit__card-logo" src="@/assets/img/clock-ico.svg" alt="clock ico">
          <h3 class="benefit__card-title">Соблюдаем договоренности и сроки</h3>
          <p class="benefit__card-text">
            Работаем по договору или оферте. Ежедневно на связи. Кошки не болеют, девушки не бросают, в отпуск и декрет не уходим.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.benefits {
  padding-top: 89px;
  padding-bottom: 111px;
  background-color: $section-bg-dark;
}
.benefits__cards {
  display: flex;
  justify-content: space-between;
  .benefit__card {
    max-width: 280px;
    &--small {
      max-width: 245px;
    }
    &-logo {
      padding-bottom: 29px;
    }
    &-title {
      font-weight: 800;
      font-size: 20px;
      line-height: 28px;
      padding-bottom: 26px;
    }
    &-text {
      line-height: 24px;
    }
  }
}
</style>