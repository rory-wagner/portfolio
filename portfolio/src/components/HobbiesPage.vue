<template>
  <div class="flex-container">
    <div class="left-text">
      <h1>Hobbies</h1>
      I have a wide variety of hobbies and interests.
      I have played sports most of my life and especially love playing, Basketball, Volleyball, and Ping Pong.
      Music has always been a passion of mine.
      I love listening and playing all kinds of genres of music such as: Rock, Jazz, and Funk.
      I love to play many instruments.
      My favorite to play is the drumset, although I love to play the piano and ukulele as well.
      I am a big Rush and Neil Peart fan.
    </div>
    <div class="right-picture">
      <img src="@/assets/drumset_outline.jpg" alt="Black and white drumset" style="max-width: 50vw; max-height: 40vh;"> 
    </div>
  </div>
</template>

<script>
export default {
  name: 'HobbiesPage',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component and children only -->
<style scoped>
  .flex-container{
    display: flex;
    max-height: 50vh;
    text-align: center;
  }
  .left-text{
    margin: 2em;
    flex: auto;
  }
  .right-picture{
    flex: auto;
  }

</style>
