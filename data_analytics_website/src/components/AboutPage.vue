<template>
  <div class="">
    <div class="title-about">
      About
      About about about
    </div>
    <div class="flex-container">
      <div class="left-text">
        Predictive Modeling
        MachineLearning and AI
      </div>
      <div class="right-picture">
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

  .flex-container{
    display: flex;
  }
  .left-text, .right-picture{
    flex: auto;
    text-align: center;
  }

</style>
