<template>
  <section class="hero">
    <img src="~/assets/photo.jpg" alt="a man smiling" class="hero__image">
    <div class="hero__bio">
      <h2>Тимошенко Константин</h2>
      <h3>Фронтенд-разработчик</h3>
      <p class="basic-info">
        Привет! Я занимаюсь разработкой современных веб приложений
      </p>
      <nav>
        <nuxt-link to="/about" class="nav__link nav__link--btn">Подробнее...</nuxt-link>
        <nuxt-link to="/contacts" class="nav__link nav__link--btn">Контакты</nuxt-link>
      </nav>
    </div>
  </section>
</template>


<style lang="scss" scoped >

.hero {
  // height: 860px;
  display: grid;
  grid-template-columns: repeat(12,minmax(10px,1fr));
  grid-column-gap: 12px;
}

.hero__image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  grid-column: 1 / span 5;
  padding: 100px 0;
}

.hero__bio {
  grid-column: 7 / span 6;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

h2 {
  font-size: 4rem;
  color: var(--dark-grey);
  margin-bottom: .785em;
  position: relative;
}

h2::before {
  content: "";
  width: 100px;
  height: 4px;
  position: absolute;
  background: #333;
  left: -135px;
  top: 30px; 
}

h3 {
  font-size: 2.2rem;
}

.basic-info {
  font-size: 1.5rem;
  line-height: 155%;
  padding-block: 2em;
}

nav {
  display: flex;
  justify-content: flex-start;
}


</style>