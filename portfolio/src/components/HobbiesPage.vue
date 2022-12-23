<template>
  <div>
    <h1>Hobbies</h1>
    <div class="flex-container">
      <div class="left-text">
        I have a wide variety of hobbies and interests.
        I have played sports most of my life and especially love playing, Basketball, Volleyball, and Ping Pong.
        Music has always been a passion of mine. I love listening to all kinds of genres of music such as: Rock, Jazz, and Funk.
        I love to play many instruments. My favorite to play is the drumset, although I love to play the piano and ukulele as well.
      </div>
      <div class="right-picture">
        <!-- need pictures here -->
        Lorem Ipsum
        Lorem Ipsum      Lorem Ipsum
        Lorem Ipsum      Lorem Ipsum
        Lorem Ipsum      Lorem Ipsum
        Lorem Ipsum      Lorem Ipsum
        Lorem Ipsum
      </div>
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
    height: 100vh;
  }
  .left-text{
    flex: auto;
  }
  .right-picture{
    flex: auto;
  }

</style>
