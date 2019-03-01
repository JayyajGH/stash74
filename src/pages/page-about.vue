<template>
  <div>
    <header>
      <nav class="site-nav">
        <a href="/">
          <img src="~/assets/images/logo.svg" class="logo"/>
				</a>
      </nav>
  	</header>

    <main>
      <h1 class="heading1 heading">about</h1>

      <section class="section">
        Blah blah blah
      </section>
    </main>
  </div>
</template>

<script>
  export default {
    name: 'PageAbout'
  };
</script>

<style scoped lang="scss">
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
