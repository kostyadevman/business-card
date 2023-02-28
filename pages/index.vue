<template>
  <section class="hero">
    <img src="~/assets/photo.jpg" alt="a man smiling" class="hero__image">
    <div class="hero__bio">
      <p class="hero__name">Тимошенко Константин</p>
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
  display: grid;
  grid-gap: 10%;
  grid-template-columns: 45% 45%;
  grid-template-rows: auto;

  @include mobile {
    grid-template-columns: 100%;
  }
}

.hero__image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  padding: 100px 0;

  @include tablet {
    padding: 15px 0;
  }

  @include mobile {
    padding: 0;
  }

}

.hero__bio {
  display: flex;
  flex-direction: column;
  justify-content: center;

  @include mobile {
    text-align: center;
  }
}

.hero__name {
  position: relative;
  margin-bottom: .785em;
  font-weight: bold;
  font-size: 3.7rem;
  color: var(--dark-grey);

  @include tablet {
    font-size: 1.8rem;
  }

  @include mobile {
    font-size: 2rem;
  }

}

.hero__name::before {
  content: "";
  width: 100px;
  height: 4px;
  position: absolute;
  background: #333;
  left: -135px;
  top: 30px; 


  @include tablet {
    width: 70px;
    height: 3px;
    left: -90px;
    top: 30px;
  }

  @include mobile {
    display: none;
  }
}

h3 {
  font-size: 2.2rem;

  @include tablet {
    font-size: 1.2rem;
  }
  @include mobile {
    font-size: 1.4rem;
  }
}

.basic-info {
  font-size: 1.5rem;
  line-height: 155%;
  padding-block: 2em;
  
  @include tablet {
    font-size: 1rem;
  }
  @include mobile {
    font-size: 1.2rem;
  }
}


</style>