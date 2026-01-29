<template>
  <div id="theatrePage" class="theatre-page">
    <div class="text-overlay">
      <div class="theatre-header-div">
        <h1>Theatre</h1>
      </div>

      <div>
        <div>
          <p>
            I love to act!
            I've been in theatre since high school.
            I have had the privilege of being in amazing musicals like Joseph and the Amazing Technicolor Dreamcoat, The Man of La Mancha, Fiddler on the Roof, Bonnie and Clyde, and She Loves Me.
            Being in theatre gives me a chance to express a character's story while being a part of an amazing team.
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
    padding: 24px;
    margin-bottom: 2rem;
    background: rgba(255,255,255,0.02);
    border-radius: 12px;
    box-shadow: 0 6px 18px rgba(2,6,23,0.6);
    box-sizing: border-box;
    overflow: hidden;
  }
  .text-overlay{
    margin-left: auto;
    margin-right: auto;
    width: 100%;
    max-width: 100%;
    text-align: center;
    box-sizing: border-box;
  }

  .theatre-img-div{
    display: flex;
    gap: 12px;
    flex-wrap: wrap;
    justify-content: center;
    margin-left: auto;
    margin-right: auto;
  }

  .mobile-br{
    display: none;
  }
  .picture{
    display: block;
    max-width: 160px;
    width: 100%;
    height: auto;
    margin: 12px;
    object-fit: contain;
    border-radius: 6px;
  }
  @media screen and (max-width: 800px) {
    .text-overlay{
      width: 100%;
      padding-bottom: 2em;
    }
    .picture{
      max-width: 120px;
    }
  }

</style>
