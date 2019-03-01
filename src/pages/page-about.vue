<template>
  <div>
    <h1 class="heading1 heading">about</h1>

    <section class="section">
      Blah blah blah
    </section>
  </div>
</template>

<script>
  export default {
    layout: 'default-page',
    name: 'PageAbout'
  };
</script>

<style scoped lang="scss">
  /* Use perfect fourth modular scale */
  .heading1 {
    font-size: 2.369rem;
    font-weight: 700;
    margin-bottom: 2rem;
  }

  .heading2 {
    font-size: 1.777rem;
    font-weight: 700;
    margin-bottom: 1rem;
  }

  .heading {
    background-color: rgb(244, 66, 69);
    color: #FFF;
  }

  .subheading {
    color: rgb(244, 66, 69);
  }

  .section {
    border: 3px solid rgb(244, 66, 69);
    border-radius: 3px;
    width: auto;
    margin: 0 auto;
    padding: 2rem;
    margin-bottom: 2rem;
  }

  @media (min-width: 800px) {
    .section {
      max-width: 800px;
    }
  }
</style>
