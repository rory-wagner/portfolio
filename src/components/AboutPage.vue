<template>
  <div class="about-page">
    <div class="flex-container">
      <div class="left-text">
        <div class="title-about">
          <h1>About Me</h1>
        </div>
        <p>
          My name is Rory Wagner and I am a software enthusiast.
          I am a Software Engineer and currently a Game Developer for my own LLC, Wagner Gaming.
          I have many interests besides just computing.
          These interests include, but are not limited to, Volleyball, Magic the Gathering, Music, and Drama.
          I have always been curious about AI, Machine Learning, and Neural Networks.
          I also enjoy learning about Cryptography and System Architecture.
        </p>
      </div>
      <div class="right-text">
        <img src="@/assets/rory_1.jpg" alt="Rory Wagner" style="max-width: 50vw; max-height: 72vh;"> 
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
  p{
    text-align: initial;
  }
  .about-page{
    margin-top: 2em;
    margin-bottom: 2em;
    max-height: 72vh;
  }

  .flex-container{
    display: flex;
    max-width: 75vw;
    margin-left: auto;
    margin-right: auto;
  }
  .left-text, .right-text{
    flex: auto;
    text-align: center;
  }

  .left-text{
    margin: 0em 2em 2em 2em;
  }

  @media screen and (max-width: 800px) {
    .flex-container{
      display: block;
      max-width: 100vw;
    }
    .about-page{
      max-height: 100%;
    }
  }

</style>
