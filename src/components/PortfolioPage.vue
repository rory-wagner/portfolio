<template>
  <div class="portfolio-page">
    <div class="text-overlay">
      <div class="portfolio-header-div">
        <h1>Portfolio</h1>
      </div>

      <div>
        <div>
          <p>
            I'm a Software Engineer currently working for my own LLC, Wagner Gaming.
            I am always on the lookout for a role in backend development.
            I have experience in quite a few backend languages, but my favorites are: Go, Python, and C#.
            I have used many other languages as shown in the rest of my portfolio and throughout this web app which I have left as a public repository that anyone can clone for their own portfolio.
            I have worked on teams that have used both Scrum and Kanban as their workflow management methodologies.
            I've graduated from Dixie State University with a bachelor's in Computer Science, and that was where I learned about my love for the technical field.
            Please checkout my <a href="https://github.com/rory-wagner">Github</a> portfolio.
          </p>
        </div>
        <div class="portfolio-img-div">
          <img src="@/assets/github_logo.png" alt="Github logo" class="picture">
        </div>
        <div>
          <p>
            I have used many different technologies over my educational and professional career, including Go, C#/.NET, and Python and this portfolio website is written in Vue.
            I have also been currently working in Godot which has been an impressive open source game engine and language.
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
    padding-top: 2em;
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
    margin: 2vw auto 2vw auto;
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
