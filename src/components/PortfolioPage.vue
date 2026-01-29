<template>
  <div id="portfolioPage" class="portfolio-page">
    <div class="text-overlay">
      <div class="portfolio-header-div">
        <h1>Portfolio</h1>
      </div>

      <div>
        <div>
          <p>
            I'm a Software Engineer currently working for my own LLC, Wagner Gaming.
            I am also a Software Engineer working at Vasion.
            I have experience in quite a few backend languages, but my favorites are: Go, Python, and C#.
            I have used many other languages as shown in the rest of my portfolio and throughout this web app which I have left as a public repository.
            This is so anyone can take this repository as a template and learn to make it their own.
            I love to share knowledge! <br/>
            I have worked on teams that have used both Scrum and Kanban as their workflow management methodologies.
            I've graduated from Dixie State University with a bachelor's in Computer Science, and that was where I learned about my love for the technology field.
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
    padding: 28px;
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

  .portfolio-img-div{
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
    }
    .picture{
      max-width: 120px;
      margin: 8px;
    }
  }

</style>
