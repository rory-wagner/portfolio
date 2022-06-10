<template>
  <div>
    <div id="top-bar">
      <img>
      <h2>
        Website Title
      </h2>
    </div>
    <div id="links-bar">
      <a class="links" style="flex-grow: 3">About</a>
      <a class="links">Portfolio</a>
      <a class="links" style="flex-grow: 3">Contact</a>
    </div>
  </div>
</template>



<script>

export default {
  name: "NavBar"
}
</script>

<style>

</style>

<style scoped>
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
