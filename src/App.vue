<script >

import Header from './components/Header.vue'
import PortfolioItem from './components/PortfolioItem.vue'
import SocialLink from './components/SocialLink.vue'
import Footer from './components/Footer.vue'
import contentsData from './assets/contents.json'
import NavBar from './components/NavBar.vue'
import Graphic from './components/Graphic.vue'

export default {
  data() {
    return {
      contents: contentsData,
    };
  },
  components: {
    Header,
    PortfolioItem,
    SocialLink,
    Footer,
    NavBar,
    Graphic,
  },
};

</script> 

<template>
  <main>
    <NavBar />
    <Header />

    <div id="works" class="row">
      <div class="col-12 col-md-3" v-for="work in contents.works" :key="work.id">
         <PortfolioItem 
          :title="work.title"
          :abstract="work.description"
          :imageUrl="work.image_thumbnail"
        />
      </div>
    </div>

    <Graphic/>
     <div id="Graphic" class="row">
        <div class="col-12 col-md-3" v-for="work in contents.graphic" :key="work.id">
           <PortfolioItem 
            :title="work.title"
            :abstract="work.description"
            :imageUrl="work.image_thumbnail"
          />
        </div>
      </div>


    <div id="social-links" class="row">
      <ul>
        <li v-for="link in contents.social_links" :key="link.id">
          <SocialLink 
            :id="link.id"
            :name="link.name"
            :url="link.url"
          />
        </li>
      </ul>
    </div>
    <Footer/>
  </main>
</template>

<style scoped>


NavBar{
  background-color: rgb(213, 173, 156);
  height: 4rem;
}

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
