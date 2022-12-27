<template>
  <div class="about-page">
    <div class="flex-container">
      <div class="left-text">
        <div class="title-about">
          <h1>About Me</h1>
        </div>
        Hello! My name is Rory Wagner and I am a software enthusiast.
        I am a Software Engineer at Vasion and I live near its headquarters in Saint George, Utah.
        I have many interests besides just software.
        These interests include, but are not limited to, Volleyball, Magic the Gathering, and Music.
        I have always been curious about AI, Machine Learning, and Neural Networks.
        I am currently taking a class at Utah Tech University to further my knowledge in Machine Learning.
      </div>
      <div class="right-text">
        <img src="@/assets/rory_1.jpg" alt="Rory Wagner" style="max-width: 50vw"> 
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AboutPage',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component and children only -->
<style scoped>
  .about-page{
    height: 100vh;
  }

  .flex-container{
    display: flex;
  }
  .left-text, .right-text{
    flex: auto;
    text-align: center;
  }

  .left-text{
    margin: 2em;
  }

</style>
