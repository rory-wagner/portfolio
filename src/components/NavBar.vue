<template>
  <header class="nav-root">
    <div class="nav-fixed">
      <div class="nav-inner">
        <div class="brand">Rory Wagner</div>

        <button
          class="hamburger"
          @click="toggleMenu"
          :aria-expanded="isOpen"
          aria-controls="nav-links"
          aria-label="Toggle navigation"
        >
          <span class="bar"></span>
          <span class="bar"></span>
          <span class="bar"></span>
        </button>

        <nav id="nav-links" class="links" :class="{ open: isOpen }">
          <a class="link" href="#aboutPage" @click="closeMenu">About</a>
          <a class="link" href="#portfolioPage" @click="closeMenu">Career</a>
          <a class="link" href="#hobbiesPage" @click="closeMenu">Hobbies</a>
          <a class="link" href="#theatrePage" @click="closeMenu">Theatre</a>
        </nav>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return { isOpen: false };
  },
  methods: {
    toggleMenu() {
      this.isOpen = !this.isOpen;
    },
    closeMenu() {
      this.isOpen = false;
    }
  }
}
</script>

<style scoped lang="scss">
@import './../assets/variables.scss';

.nav-root{ width: 100%; }
.nav-fixed{
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 50;
  background: linear-gradient(180deg, rgba(11,18,32,0.9), rgba(11,18,32,0.75));
  backdrop-filter: blur(6px);
  border-bottom: 1px solid rgba(255,255,255,0.03);
}

.nav-inner{
  height: 72px;
  max-width: 1100px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 20px;
  gap: 12px;
}

.brand{
  font-weight: 700;
  color: var(--ivory);
  font-size: 1.05rem;
}

.links{
  display: flex;
  gap: 12px;
  align-items: center;
}

.link{
  color: var(--muted-slate);
  text-decoration: none;
  padding: 8px 12px;
  border-radius: 8px;
  transition: color .15s ease, background .15s ease, transform .05s ease;
  font-weight: 600;
}

.link:hover{
  color: var(--ivory);
  background: rgba(255,255,255,0.03);
  transform: translateY(-1px);
}

/* Hamburger button (hidden on wide screens) */
.hamburger{
  display: none;
  position: relative;
  width: 40px;
  height: 36px;
  padding: 4px;
  background: transparent;
  border: 0;
  border-radius: 8px;
  cursor: pointer;
  align-items: center;
  justify-content: center;
  overflow: visible;
}

.hamburger .bar{
  position: absolute;
  left: 8px;
  right: 8px;
  height: 2px;
  background: var(--ivory);
  border-radius: 2px;
  transition: transform .22s ease, opacity .18s ease, top .22s ease;
  transform-origin: center;
}

.hamburger .bar:nth-child(1){ top: 9px; }
.hamburger .bar:nth-child(2){ top: 16px; }
.hamburger .bar:nth-child(3){ top: 23px; }

.hamburger:hover,
.hamburger:focus{
  background: rgba(255,255,255,0.04);
}

.hamburger:focus{
  outline: 2px solid rgba(255,255,255,0.06);
  outline-offset: 2px;
}

.hamburger[aria-expanded="true"] .bar:nth-child(1){
  top: 16px;
  transform: rotate(45deg);
}
.hamburger[aria-expanded="true"] .bar:nth-child(2){
  opacity: 0;
}
.hamburger[aria-expanded="true"] .bar:nth-child(3){
  top: 16px;
  transform: rotate(-45deg);
}

@media (max-width: 720px){
  .nav-inner{ padding: 0 12px; }

  .links{
    display: none;
    position: absolute;
    top: 72px;
    left: 0;
    right: 0;
    flex-direction: column;
    background: linear-gradient(180deg, rgba(11,18,32,0.95), rgba(11,18,32,0.95));
    padding: 12px 16px;
    gap: 6px;
    border-bottom: 1px solid rgba(255,255,255,0.02);
    z-index: 49;
  }

  .links.open{
    display: flex;
  }

  .link{
    display: block;
    padding: 10px 12px;
    border-radius: 6px;
  }

  .hamburger{ display: flex; }
}

</style>
