<template>
  <section class="comparison">
    <div class="container">
      <div class="comparison__title">Сравните</div>
      <table class="comparison__table">
        <tr class="comparison__table-row">
          <th></th>
          <th class="comparison__table-head-cell">
            Исполнитель idPowers
            <img class="comparison__table-choice" src="@/assets/img/choice-ico.svg" alt="">
          </th>
          <th class="comparison__table-head-cell">Штатный исполнитель</th>
          <th class="comparison__table-head-cell">Фрилансер</th>
        </tr>
        <tr class="comparison__table-row">
          <td class="comparison__table-cell comparison__table-cell-item">Время на поиск подходящего кандидата</td>
          <td class="comparison__table-cell">1-2 недели</td>
          <td class="comparison__table-cell">1-3 месяца</td>
          <td class="comparison__table-cell">1-3 месяца</td>
        </tr>
        <tr class="comparison__table-row">
          <td class="comparison__table-cell comparison__table-cell-item">Оплата рекрутинговому агентству</td>
          <td class="comparison__table-cell">Отсутствуют</td>
          <td class="comparison__table-cell">Высокая</td>
          <td class="comparison__table-cell">Отсутствуют</td>
        </tr>
        <tr class="comparison__table-row">
          <td class="comparison__table-cell comparison__table-cell-item">Гарантия качества</td>
          <td class="comparison__table-cell">
            <img class="confirm-img" src="@/assets/img/yes-ico.svg" alt="">
          </td>
          <td class="comparison__table-cell">
            <img class="confirm-img" src="@/assets/img/no-ico.svg" alt="">
          </td>
          <td class="comparison__table-cell">
            <img class="confirm-img" src="@/assets/img/no-ico.svg" alt="">
          </td>
        </tr>
        <tr class="comparison__table-row">
          <td class="comparison__table-cell comparison__table-cell-item">Вероятность ошибиться с исполнителем</td>
          <td class="comparison__table-cell">Очень низкая</td>
          <td class="comparison__table-cell">Средняя</td>
          <td class="comparison__table-cell">Очень высокая</td>
        </tr>
        <tr class="comparison__table-row">
          <td class="comparison__table-cell comparison__table-cell-item">Предварительно отобранные и проверенные кандидаты</td>
          <td class="comparison__table-cell">
            <img class="confirm-img" src="@/assets/img/yes-ico.svg" alt="">
          </td>
          <td class="comparison__table-cell">
            <img class="confirm-img" src="@/assets/img/no-ico.svg" alt="">
          </td>
          <td class="comparison__table-cell">
            <img class="confirm-img" src="@/assets/img/no-ico.svg" alt="">
          </td>
        </tr>
        <tr class="comparison__table-row">
          <td class="comparison__table-cell comparison__table-cell-item">Расходы на прекращение работы (увольнение)</td>
          <td class="comparison__table-cell">Отсутствуют</td>
          <td class="comparison__table-cell">Очень высокие</td>
          <td class="comparison__table-cell">Отсутствуют</td>
        </tr>
        <tr class="comparison__table-row">
          <td class="comparison__table-cell comparison__table-cell-item">Бесплатный тестовый период</td>
          <td class="comparison__table-cell">
            <img class="confirm-img" src="@/assets/img/yes-ico.svg" alt="">
          </td>
          <td class="comparison__table-cell">
            <img class="confirm-img" src="@/assets/img/no-ico.svg" alt="">
          </td>
          <td class="comparison__table-cell">
            <img class="confirm-img" src="@/assets/img/no-ico.svg" alt="">
          </td>
        </tr>
        <tr class="comparison__table-row">
          <td class="comparison__table-cell comparison__table-cell-item">Стоимость услуг</td>
          <td class="comparison__table-cell comparison__table-cell--primary">$$$$</td>
          <td class="comparison__table-cell comparison__table-cell--danger">$$$$$</td>
          <td class="comparison__table-cell comparison__table-cell--danger">$$$</td>
        </tr>
      </table>
    </div>
  </section>
</template>

<style lang="scss">
.comparison {
  background-color: $section-bg-dark;
  padding-top: 97px;
  padding-bottom: 83px;
  &__title {
    font-weight: 800;
    font-size: 48px;
    line-height: 59px;
    text-align: center;
    padding-bottom: 88px;
  }
  &__table {
    border-collapse: collapse;
    width: 100%;
  }
  &__table-row:nth-child(odd) {
    height: 108px;
  }
  &__table-row:nth-child(even) {
    height: 80px;
    background-color: $light-color;
  }
  &__table-head-cell {
    font-weight: 800;
    font-size: 20px;
    line-height: 28px;
    text-align: left;
    padding-right: 40px;
    max-width: 200px;
  }
  &__table-cell {
    font-weight: 500;
    font-size: 18px;
    line-height: 28px;
  }
  &__table-choice {
    padding-top: 8px;
  }
  &__table-cell--primary {
    color: $main-color;
  }
  &__table-cell--danger {
    color: $danger-color;
  }
  &__table-cell-item {
    font-weight: 600;
    max-width: 325px;
    padding-left: 40px;
    padding-right: 95px;
  }
}
</style>