<template>
  <div class="flex-container">
    <div class="left-text">
      <h1>Hobbies</h1>
      <p>
        I have a wide variety of hobbies and interests.
        I have played sports most of my life and especially love playing, Basketball, Volleyball, Pickleball, and Ping Pong.
      </p>
      <p>
        Music has always been a passion of mine.
        I love listening and playing all kinds of genres of music such as: Rock, Jazz, and Funk.
        My favorite instrument to play is the drumset, although I love to play the piano, bass, and ukulele as well.
        My three favorite bands to listen to right now are Dirty Loops, Rush, and Volbeat.
      </p>
    </div>
    <div class="right-picture">
      <img src="@/assets/drumset_outline.jpg" alt="Black and white drumset" style="max-width: 50vw; max-height: 40vh;" class="picture"> 
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
  p{
    text-align: initial;
  }
  .flex-container{
    display: flex;
    text-align: center;
    max-width: 75vw;
    margin-left: auto;
    margin-right: auto;
  }
  .left-text{
    margin: 0em 2em 2em 2em;
    flex: auto;
  }
  .right-picture{
    margin: 2em 0em 0em 0em;
    flex: auto;
  }
  @media screen and (max-width: 900px) {
    .picture{
      display: none;
    }
  }

  @media screen and (max-width: 800px) {
    .flex-container{
      display: block;
    }
  }

</style>
