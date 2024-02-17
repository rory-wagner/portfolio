<template>
  <div class="theatre-page">
    <div class="text-overlay">
      <div class="theatre-header-div">
        <h1>Theatre</h1>
      </div>

      <div>
        <div>
          <p>
            I love to act!
            I've been in theatre since high school.
            I have been in She Loves Me, Fiddler on the Roof, and Joseph and the Amazing Technicolor Dreamcoat.
            Being in theatre gives me a chance to express a character's story.
            My favorite part of theatre is the great amount of energy that goes into the atmosphere.
          </p>
        </div>
        <div class="theatre-img-div">
          <img src="@/assets/she_loves_me.jpg" alt="She Loves Me Cover" class="picture">
          <img src="@/assets/joseph_dreamcoat.jpg" alt="Joseph and the Amazing Technicolor Dreamcoat Cover" class="picture">
          <img src="@/assets/fiddler.jpg" alt="Fiddler on the Roof Cover" class="picture">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TheatrePage',
  computed: {
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component and children only -->
<style scoped lang="scss">
  @import './../assets/variables.scss';

  p{
    text-align: initial;
  }
  .theatre-page{
    background-color: $primary-blue;
  }
  .text-overlay{
    margin-left: auto;
    margin-right: auto;
    width: 75vw;
    text-align: center;
  }

  .theatre-img-div{
    display: flex;
    margin-left: auto;
    margin-right: auto;
  }

  .mobile-br{
    display: none;
  }
  .picture{
    max-width: 20vw;
    max-height: 25vh;
    margin: 1vw;
  }
  @media screen and (max-width: 800px) {
    .text-overlay{
      width: 90vw;
      padding-bottom: 2em;
    }
    .picture{
      display: none;
    }
  }

</style>
