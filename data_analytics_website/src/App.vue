<template>
  <NavBar
    id="navbar"
  />
  <MainHome
    id="mainhome"
  />
  <BelowHome
    id="belowHome"
  />
  <AboutPage
    id="aboutPage"
  />
  <ContactPage
    id="contactPage"
  />
</template>

<script>
import NavBar from './components/NavBar.vue'
import MainHome from './components/MainHome.vue'
import BelowHome from './components/BelowHome.vue'
import AboutPage from './components/AboutPage.vue'
import ContactPage from './components/ContactPage.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    MainHome,
    BelowHome,
    AboutPage,
    ContactPage,
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
