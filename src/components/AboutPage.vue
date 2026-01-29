<template>
  <div id="aboutPage" class="about-page">
    <div class="flex-container">
      <div class="left-text">
        <div class="title-about">
          <h1>About Me</h1>
        </div>
        <p>
          Hi! I'm Rory Wagner and I am a software enthusiast.
          I am a Software Engineer and currently a Game Developer for my own LLC, Wagner Gaming.
          I have always enjoyed learning about AI, Security, and Cryptography.
          These fields have always fascinated me and I love to educate myself on all the little details that go into making them work.
          I have many hobbies besides just computing.
          These hobbies include, but are not limited to, Volleyball, Magic the Gathering, Music, and Drama.
        </p>
      </div>
      <div class="right-text">
        <img src="@/assets/rory_1.jpg" alt="Rory Wagner" class="profile-img">
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
      padding: 28px;
      background: rgba(255,255,255,0.02);
      border-radius: 12px;
      box-shadow: 0 6px 18px rgba(2,6,23,0.6);
      box-sizing: border-box;
      overflow: hidden;
    }

    .flex-container{
      display: flex;
      align-items: center;
      gap: 24px;
      max-width: 100%;
      margin-left: auto;
      margin-right: auto;
      box-sizing: border-box;
    }

    .left-text{
      flex: 0 1 60%;
      text-align: left;
      box-sizing: border-box;
      padding-right: 12px;
    }

    .right-text{
      flex: 0 1 36%;
      display: flex;
      align-items: center;
      justify-content: center;
      box-sizing: border-box;
    }

  @media screen and (max-width: 800px) {
    .flex-container{
      flex-direction: column;
      align-items: stretch;
      max-width: 100vw;
    }
    .left-text{
      flex: none;
      order: 0;
      text-align: left;
      padding: 0 4px 12px 4px;
    }
    .right-text{
      flex: none;
      order: 1;
      padding: 0 4px;
    }

    .about-page{
      padding: 18px;
      margin-top: 1rem;
    }
  }

  .profile-img{
    display: block;
    width: 100%;
    height: auto;
    max-width: 380px;
    max-height: 420px;
    border-radius: 8px;
    object-fit: cover;
  }

</style>
