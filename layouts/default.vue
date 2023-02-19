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
  display: flex;
  justify-content: flex-start;
}

.nav__link {
  display: inline;
  width: 100%;
  max-width: 200px;
  padding: .785em 2em;
  font-weight: bold;
  font-size: .725rem;
  color: #999;
  text-decoration: none;
  text-transform: uppercase;

  &--btn {
    text-align: center;
    margin-right: 12px;
    max-width: 125px;
    border: 1px solid var(--light-grey);
    border-radius: 100px;
    &:hover {
      border: 1px solid var(--accent);
    }
  }
  
  &:hover {
    color: var(--accent);
  }
}

</style>