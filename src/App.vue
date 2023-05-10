<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import PortfolioItem from './components/PortfolioItem.vue'
</script>

<template>
  <header class="mb-4">
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="custom message" />
    </div>
  </header>

  <main>
    <div class="row">
      <div class="col">
        <PortfolioItem 
          title="news 1"
          abstract="Lorem ipsum dolor sit amet, consectetur adipiscing elit."
          imageUrl="https://source.unsplash.com/random/?green"
        />

      </div>
      <div class="col">
        <PortfolioItem 
          title="news 2"
          abstract="Cras justo odio, dapibus ac facilisis in, egestas eget quam."
          imageUrl="/images/image1.jpg"
        />
      </div>
    </div>
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
