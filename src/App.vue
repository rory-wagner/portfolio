<template>
  <div id="app-root">
    <NavBar />
    <main class="container">
      <div class="mainView">
        <AboutPage />
        <PortfolioPage />
        <HobbiesPage />
        <TheatrePage />
      </div>
    </main>
  </div>
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
<style lang="scss">
@import './assets/variables.scss';

html, body, #app{
  height: 100%;
}
body{
  margin: 0;
  font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
  background: var(--bg);
  color: var(--text);
}

.container{
  max-width: 1100px;
  margin: 0 auto;
  padding: 96px 20px 48px; // leave space for nav
}

.mainView{
  display: flex;
  flex-direction: column;
  gap: 48px;
}

h1, h2, h3{
  color: var(--ivory);
  margin: 0 0 12px 0;
}

p{ line-height: 1.6; color: var(--muted); }

/* Apply single band background to each section (direct children of .mainView) */
.mainView > *{
  background-color: var(--band);
  border-radius: 12px;
  padding: 28px;
  box-sizing: border-box;
  /* make anchored sections stop below the fixed navbar */
  scroll-margin-top: calc(var(--nav-height) + 8px);
}

html {
  scroll-behavior: smooth;
}
</style>
