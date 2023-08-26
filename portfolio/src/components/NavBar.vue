<template>
  <div id="navbar">
    <div id="nav-fixed">
      <div id="top-bar">
        <!-- <img> -->
        <h2>
          Rory Wagner
        </h2>
      </div>
      <!-- <hr> -->
      <div id="links-bar">
        <a class="a-links" href="#aboutPage">
          <input class="input-links" type="button" value="About">
        </a>
        <a class="a-links" href="#portfolioPage">
          <input class="input-links" type="button" value="Professional Portfolio">
        </a>
        <a class="a-links" href="#hobbiesPage">
          <input class="input-links" type="button" value="Hobbies">
        </a>
      </div>
    </div>

    <div id="nav-space">
    </div>
  </div>
</template>

<script>
//need to use fixed position for the navbar
export default {
  name: "NavBar"
}
</script>

<style>

</style>

<style scoped lang="scss">
  @import './../assets/variables.scss';

  .navbar{
    background-color: $primary-green;
  }

  #nav-space{
    height: 120px;
  }

  #nav-fixed{
    position: fixed;
    width: 100%;
    z-index: 10;
    background-color: $primary-green;
  }
  #top-bar{
    width: 100%;
    text-align: center;
  }

  #links-bar{
    display: flex;
    flex-direction: row;
    width: 100%;
  }

  .input-links{
    width: 100%;
    text-align: center;
  }

  .a-links{
    width: 100%;
  }
</style>
