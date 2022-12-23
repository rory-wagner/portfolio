<template>
  <NavBar
    id="navbar"
  />
  <!-- might add a side bar here -->
  <AboutPage
    id="aboutPage"
  />
  <PortfolioPage
    id="mainhome"
  />
  <HobbiesPage
    id="belowHome"
  />
  <!-- <ContactPage
    id="contactPage"
  /> -->
</template>

<script>
import NavBar from './components/NavBar.vue'
import PortfolioPage from './components/PortfolioPage.vue'
import HobbiesPage from './components/HobbiesPage.vue'
import AboutPage from './components/AboutPage.vue'

export default {
  name: 'App',
  components: {
    NavBar,
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
  #navbar{
    
  }
  #mainhome{

  }
  #belowHome{
    
  }
</style>
