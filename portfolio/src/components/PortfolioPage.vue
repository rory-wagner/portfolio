<template>
  <div>
    <div id="text-overlay">
      <div>
        <h1>Portfolio</h1>
      </div>

      <div>
        <div>
          I'm a Software Engineer currently working at Vasion.
          I've graduated from Dixie State University with a bachelor's in Computer Science and enjoy everything tech related.
          I have used many software development languages as shown in the rest of my portfolio and throughout this whole web app.
          I have a few Git portfolios in various git version control services including  <a href="https://github.com/rory-wagner">Github</a> and <a href="https://gitlab.com/ro_boat">Gitlab</a>.
        </div>
        <div>
          <img src="@/assets/github_logo.png" alt="Github logo" style="max-width: 20vw"> 
          <img src="@/assets/gitlab_logo.png" alt="Gitlab logo" style="max-width: 20vw">
        </div>
        <div>
          I have used many different technologies over my educational and professional career, including Go, C#/.NET, and Python and this portfolio website is written in Vue.
        </div>
        <img src="@/assets/golang.jpg" alt="Golang" style="max-width: 20vw; max-height: 20vh;">
        <img src="@/assets/Csharp.png" alt="C#" style="max-width: 20vw; max-height: 20vh;">
        <img src="@/assets/python.png" alt="Python" style="max-width: 20vw; max-height: 20vh;">
        <img src="@/assets/logo.png" alt="Vue" style="max-width: 20vw; max-height: 20vh;">
      </div>

      <!-- include pictures at the bottom here -->

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
<style scoped>

  #text-overlay{
    background-size: cover;
    background-repeat: no-repeat;
    text-align: center;
    max-height: 55vh;
    margin: 4em;
  }

</style>
