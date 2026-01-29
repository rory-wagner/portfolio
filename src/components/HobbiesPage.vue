<template>
  <div id="hobbiesPage" class="flex-container">
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
        I'm not a Spotify influencer by any means, but you can check out my public playlists <a href="https://open.spotify.com/user/rory.wagner">here</a> if you need something new to listen to.
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
    max-width: 100%;
    margin-left: auto;
    margin-right: auto;
    gap: 20px;
    flex-wrap: wrap;
    padding: 24px;
    background: rgba(255,255,255,0.02);
    border-radius: 12px;
    box-shadow: 0 6px 18px rgba(2,6,23,0.6);
    box-sizing: border-box;
    overflow: hidden;
  }
  .left-text{
    margin: 0;
    flex: 1 1 320px;
  }
  .right-picture{
    margin: 0;
    flex: 1 1 240px;
  }
  @media screen and (max-width: 900px) {
    .picture{
      max-width: 100%;
      height: auto;
      display: block;
    }
  }

  @media screen and (max-width: 800px) {
    .flex-container{
      display: block;
    }
  }

  .picture{
    display: block;
    max-width: 100%;
    width: 100%;
    height: auto;
    border-radius: 8px;
    object-fit: cover;
  }

</style>
