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
      <h1 class="heading1 heading">contact</h1>

      <section class="section">
        <h2 class="heading2 subheading">Contact details</h2>
        <address>
          <p>1 Court Close, Horfield, Bristol BS7 0XH</p>
          <div>
            <a href="mailto:hello@stash74.co.uk">hello@stash74.co.uk</a>
          </div>
          <div>
            <a href="tel:+447973864573">0797 3864573</a>
          </div>
        </address>
      </section>

      <section class="section">
        <form>
          <fieldset>
            <legend class="heading2 subheading">Send us a message</legend>
            <div>
              <label for="name">Name:</label>
              <input id="name" type="text">
            </div>

            <div>
              <label for="email">Email:</label>
              <input id="email" type="text">
            </div>

            <div>
              <label for="message">Message:</label>
              <input id="message" type="text">
            </div>
          </fieldset>

          <input type="submit" value="send request" />
        </form>
        Add reCAPTCHAv3
      </section>
    </main>
  </div>
</template>

<script>
  export default {
    name: 'PageContact'
  };
</script>

<style scoped lang="scss">
  .heading {
    background-color: rgb(244, 160, 65);
    color: #FFF;
  }

  .subheading {
    color: rgb(244, 160, 65);
  }

  .logo {
    height: 40px;
  }

  .section {
    border: 3px solid rgb(244, 160, 65);
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
