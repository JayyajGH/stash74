<template>
  <div>
    Add header
    <h1 class="heading1 heading">contact</h1>

    <h2 class="heading2 subheading">Contact details</h2>
    <address>
      <p>1 Court Close, Horfield, Bristol BS7 0XH</p>
      <a href="mailto:hello@stash74.co.uk">hello@stash74.co.uk</a>
      <a href="tel:+447973864573">0797 3864573</a>
    </address>

    <form>
    <fieldset>
        <legend class="heading2 subheading">Send us a message</legend>
    </fieldset>

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

    <input type="submit" value="send request" />
  </form>

    <p>
      Add reCAPTCHAv3
    </p>
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
</style>
