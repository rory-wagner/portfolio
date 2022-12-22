<template>
  <div>
    <div id="text-overlay" :style="textStyle">
      <div>
        Less but better
      </div>

      <div>
        Grow your business better while spending less on fancy titles
      </div>

      <input type="button" value="Partner with us">
    </div>

  </div>
</template>

<script>
export default {
  name: 'MainHome',
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

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  #text-overlay{
    background-image: url("@/assets/AvatarState.gif");
    background-size: cover;
    background-repeat: no-repeat;
    text-align: center;
    height: 72vw;
  }

</style>
