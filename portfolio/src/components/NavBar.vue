<template>
  <div id="navbar">

    <div id="nav-fixed">
      <div id="top-bar">
        <img>
        <h2>
          Rory Wagner
        </h2>
      </div>
      <hr>
      <div id="links-bar">
        <input class="links" type="button" value="About">
        <input class="links" type="button" value="Professional Portfolio">
        <input class="links" type="button" value="Hobbies">
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
    height: 150px;
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

  .links{
    width: 100%;
    text-align: center;
  }
</style>
