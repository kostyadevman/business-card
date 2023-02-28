<template>
    <div class="portfolio-container">
      <nuxt />
    </div>
</template>

<style lang="scss">

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --accent: #00b8ff;
  --dark-grey: #282a2b;
  --light-grey: #8d98a1;
}

body {
  font-family: 'Work Sans', sans-serif;
  font-weight: regular;
  color: var(--light-grey);
}

.portfolio-container {
  width: 1134px;
  max-width: 100%;
  margin: 0px auto;
  padding: 1.5em;
}

nav {
  font-size: 14px;
  display: flex;
  justify-content: flex-start;
  margin-right: 120px;
  
  @include tablet {
    flex-direction: column;
    margin: 0;
  }
}

.nav__link {
  display: inline;
  width: 100%;
  padding: .785em 2em;
  font-weight: bold;
  font-size: .725rem;
  color: #999;
  text-decoration: none;
  text-transform: uppercase;

  &--btn {
    text-align: center;
    border: 1px solid var(--light-grey);
    border-radius: 100px;
    &:hover {
      border: 1px solid var(--accent);
    }

    &:not(:last-child) {
      margin-right: 12px;
    }

    @include tablet {
      margin: 0 0 20px 0;
    }
  }
  
  &:hover {
    color: var(--accent);
  }
}

</style>