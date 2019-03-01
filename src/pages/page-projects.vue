<template>
  <div>
    <h1 class="heading1 heading">projects</h1>
    <section class="section">
      <h2 class="heading2 subheading">Previous projects</h2>
    </section>
    <section class="section">
      <h2 class="heading2 subheading">Need a website built?</h2>
      <p>
        Drop me a message and we can discuss your requirements
      </p>
    </section>
  </div>
</template>

<script>
  export default {
    layout: 'default-page',
    name: 'PageProjects'
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
    background-color: rgb(65, 104, 244);
    color: #FFF;
  }

  .subheading {
    color: rgb(65, 104, 244);
  }

  .section {
    border: 3px solid rgb(65, 104, 244);
    border-radius: 3px;
    width: 100%;
    margin: 0 auto;
    padding: 2rem;
    margin-bottom: 2rem;
  }

  @media (min-width: 800px) {
    .section {
      width: 800px;
    }
  }
</style>
