<template>
  <div class="contact-page">

    <div class="flex-container">
      <div class="left-text">
        Contact Us
      </div>
      <div class="right-inputs">
        <input
          placeholder="First Name"
        >
        <input
          placeholder="Last Name"
        >
        <input
          placeholder="Email"
        >
        <input
          placeholder="Phone"
        >
        <input
          placeholder="Company Name"
        >
        <input
          placeholder="Some Other Field"
        >
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

  .contact-page{
    height: 100vh;
  }

  .flex-container{
    display: flex;
  }
  .left-text, .right-inputs{
    flex: 1;
    text-align: center;
  }

</style>
