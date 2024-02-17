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
          <button class="input-links" role="button">About</button>
        </a>
        <a class="a-links" href="#portfolioPage">
          <button class="input-links" role="button">Career</button>
        </a>
        <a class="a-links" href="#hobbiesPage">
          <button class="input-links" role="button">Hobbies</button>
        </a>
        <a class="a-links" href="#theatrePage">
          <button class="input-links" role="button">Theatre</button>
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
  .input-links {
    appearance: none;
    background-color: #FAFBFC;
    border: 1px solid rgba(27, 31, 35, 0.15);
    border-radius: 6px;
    box-shadow: rgba(27, 31, 35, 0.04) 0 1px 0, rgba(255, 255, 255, 0.25) 0 1px 0 inset;
    box-sizing: border-box;
    color: #24292E;
    cursor: pointer;
    display: inline-block;
    font-family: -apple-system, system-ui, "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji";
    font-size: 14px;
    font-weight: 500;
    line-height: 20px;
    list-style: none;
    padding: 6px 16px;
    position: relative;
    transition: background-color 0.2s cubic-bezier(0.3, 0, 0.5, 1);
    user-select: none;
    -webkit-user-select: none;
    touch-action: manipulation;
    vertical-align: middle;
    white-space: nowrap;
    word-wrap: break-word;
    width: 100%;
  }

  .input-links:hover {
    background-color: #F3F4F6;
    text-decoration: none;
    transition-duration: 0.1s;
  }

  .input-links:disabled {
    background-color: #FAFBFC;
    border-color: rgba(27, 31, 35, 0.15);
    color: #959DA5;
    cursor: default;
  }

  .input-links:active {
    background-color: #EDEFF2;
    box-shadow: rgba(225, 228, 232, 0.2) 0 1px 0 inset;
    transition: none 0s;
  }

  .input-links:focus {
    outline: 1px transparent;
  }

  .input-links:before {
    display: none;
  }

  .input-links:-webkit-details-marker {
    display: none;
  }

  .a-links{
    width: 100%;
  }
</style>
