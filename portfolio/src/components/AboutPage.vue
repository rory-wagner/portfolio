<template>
  <div class="about-page">
    <div class="title-about">
      About
      About about about
    </div>
    <div class="flex-container">
      <div class="left-text">
        Predictive Modeling
        MachineLearning and AI
      </div>
      <div class="right-text">
        Marketing Analytics
        Database Engineering
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AboutPage',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
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

</style>
