<template>
<div>
  <nav>
    <nuxt-link to="/" class="nav__link">На главную</nuxt-link>
  </nav>
  <hr />
  <section class="skills">
    <h2 class="skills__title">Skills</h2>
    <ul class="skills__list">
      <li class="skills__item">разрабатываю в основном на react + redux</li>
      <li class="skills__item">умею настраивать сборку проекта с помощью webpack, vite, babel, a также настраивать линтеры - eslint и stylelint</li>
      <li class="skills__item">придерживаюсь FSD архитектуре</li>
      <li class="skills__item">могу писать unit тесты</li>
      <li class="skills__item">использую в своих проектах storybook, а для скриншотного тестирования - loki</li>
      <li class="skills__item">могу разрабатывать приложения для разных языков, используя i18next</li>
      <li class="skills__item">умею адаптивно верстать, а также использовать препроцессоры, css-модули, БЭМ</li>
      <li class="skills__item">умею работать с Figma, как разработчик</li>
      <li class="skills__item">изучаю на собственных проектах TypeScript, RTK Query, storybook, i18next, scss, loki, json-server</li>
    </ul>
  </section>
</div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.skills {
  display: flex;
  align-items: center;
  flex-direction: column;
  
  &__title {
    margin-top: 10px;
    font-size: 32px;
  }

  &__list {
    margin-top: 100px;
  }

  &__item {
    margin-bottom: 5px;
    font-size: 20px;
  }
}
</style>