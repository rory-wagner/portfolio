<template>
  <NavBar
    id="navbar"
  />
  <div class="mainView">
    <AboutPage
      id="aboutPage"
    />
    <PortfolioPage
      id="portfolioPage"
    />
    <HobbiesPage
      id="hobbiesPage"
    />
    <TheatrePage
      id="theatrePage"
    />
  </div>
  <!-- <ContactPage
    id="contactPage"
  /> -->
</template>

<script>
import NavBar from './components/NavBar.vue'
import AboutPage from './components/AboutPage.vue'
import PortfolioPage from './components/PortfolioPage.vue'
import HobbiesPage from './components/HobbiesPage.vue'
import TheatrePage from './components/TheatrePage.vue'


export default {
  name: 'App',
  components: {
    NavBar,
    TheatrePage,
    PortfolioPage,
    HobbiesPage,
    AboutPage,
  }
}
</script>

<style>
  body{
    margin: 0px;
  }
  .mainView{
    overflow-y: scroll;
    max-height: calc(100vh - 100px)
  }
  #navbar{

  }
  #portfolioPage{

  }
  #hobbiesPage{
    
  }
  html {
    scroll-behavior: smooth;
    overflow-y: hidden;
  }
</style>
