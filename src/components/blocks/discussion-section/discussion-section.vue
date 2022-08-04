<template>
  <section class="discussion">
    <div class="container">
      <h2 class="discussion__title">Давайте обсудим ваш проект</h2>
      <p class="discussion__subtitle">
        Мы заинтересованы в долгосрочном сотрудничестве. Работая с нами вы получаете надежного партнера для решения всех технических задач по вашим проектам.
      </p>
      <action-button color="light-color">Напишите нам</action-button>
    </div>
  </section>
</template>

<script>
import ActionButton from "@/components/common/buttons/ActionButton.vue";
export default {
  components: {
    ActionButton
  }
}
</script>

<style lang="scss">
.discussion {
  background-color: $main-color;
  color: $text-color-light;
  text-align: center;
  padding: 97px 0 119px 0;
  &__title {
    font-weight: 800;
    font-size: 48px;
    line-height: 59px;
    padding-bottom: 32px;
  }
  &__subtitle {
    font-weight: 500;
    font-size: 18px;
    line-height: 28px;
    max-width: 683px;
    margin: 0 auto;
    padding-bottom: 57px;
  }
}
</style>