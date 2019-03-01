<template>
  <div>
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
  </div>
</template>

<script>
  export default {
    layout: 'default-page',
    name: 'PageContact'
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
    background-color: rgb(244, 160, 65);
    color: #FFF;
  }

  .subheading {
    color: rgb(244, 160, 65);
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
