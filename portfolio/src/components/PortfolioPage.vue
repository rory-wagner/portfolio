<template>
  <div>
    <div id="text-overlay" :style="textStyle">
      <div>
        <h1>Portfolio</h1>
      </div>

      <div>
        I'm a Software Engineer currently working at Vasion.
        I've graduated from Dixie State University with a bachelor's in Computer Science and enjoy everything tech related.
        I have used many software development languages as shown in the rest of my portfolio and throughout this whole web app.
        I have a few Git portfolios in various git version control services including  <a href="https://www.w3schools.com">Github</a>,  <a href="https://www.w3schools.com">Gitlab</a>, and  <a href="https://www.w3schools.com">Azure</a>.
      </div>

      <!-- include pictures at the bottom here -->

    </div>

  </div>
</template>

<script>
export default {
  name: 'PortfolioPage',
  computed: {
    // textDisplayWidth() {
    //   let text_overlay = document.getElementById('text-overlay');
    //   console.log(text_overlay)
    //   return text_overlay.offsetWidth;
    // },
    // textStyle() { return "height: " + this.textDisplayWidth / 560 * 300 + ";" },
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component and children only -->
<style scoped>

  #text-overlay{
    /* background-image: url("@/assets/AvatarState.gif"); */
    background-size: cover;
    background-repeat: no-repeat;
    text-align: center;
    height: 72vh;
  }

</style>
