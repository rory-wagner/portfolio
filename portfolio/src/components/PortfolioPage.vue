<template>
  <div class="portfolio-page">
    <div class="text-overlay">
      <div class="portfolio-header-div">
        <h1>Portfolio</h1>
      </div>

      <div>
        <div>
          <p>
            I'm a Software Engineer currently working at Vasion.
            I've graduated from Dixie State University with a bachelor's in Computer Science and enjoy everything tech related.
            I have used many software development languages as shown in the rest of my portfolio and throughout this whole web app.
            I have a few Git portfolios in various git version control services including  <a href="https://github.com/rory-wagner">Github</a> and <a href="https://gitlab.com/ro_boat">Gitlab</a>.
          </p>
        </div>
        <div class="portfolio-img-div">
          <img src="@/assets/github_logo.png" alt="Github logo" class="picture">
          <img src="@/assets/gitlab_logo.png" alt="Gitlab logo" class="picture">
        </div>
        <div>
          <p>
            I have used many different technologies over my educational and professional career, including Go, C#/.NET, and Python and this portfolio website is written in Vue.
          </p>
        </div>
        <div class="portfolio-img-div">
          <img src="@/assets/golang.jpg" alt="Golang" class="picture">
          <img src="@/assets/Csharp.png" alt="C#" class="picture">
          <img src="@/assets/python.png" alt="Python" class="picture">
          <img src="@/assets/logo.png" alt="Vue" class="picture">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'PortfolioPage',
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
  .portfolio-page{
    margin-bottom: 2em;
    background-color: $primary-blue;
  }
  .text-overlay{
    margin-left: auto;
    margin-right: auto;
    width: 75vw;
    text-align: center;
  }

  .portfolio-img-div{
    display: flex;
    margin-left: auto;
    margin-right: auto;
  }

  .mobile-br{
    display: none;
  }
  .picture{
    max-width: 20vw;
    max-height: 20vh;
    margin: 2vw;
  }
  @media screen and (max-width: 800px) {
    .text-overlay{
      width: 90vw;
    }
    .picture{
      display: none;
    }
  }

</style>
