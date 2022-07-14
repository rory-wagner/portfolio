<template>
  <div>

    <div id="nav-fixed">
      <div id="top-bar">
        <img>
        <h2>
          Website Title
        </h2>
      </div>
      <hr>
      <div id="links-bar">
        <input class="links" type="button" value="About">
        <input class="links" type="button" value="Portfolio">
        <input class="links" type="button" value="Contact">
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

<style scoped>
  #nav-space{
    height: 120px;
  }

  #nav-fixed{
    position: fixed;
    width: 100%;
    z-index: 10;
    background-color: #326872;
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
