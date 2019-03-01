<template>
  <div>
    <header class="header">
      <nav class="site-nav">
        <a href="/">
          <img src="~/assets/images/logo.svg" class="logo"/>
				</a>
      </nav>
  	</header>
    <main>
      <nuxt />
    </main>
  </div>
</template>

<style scoped lang="scss">
/*
  :root {
    --light-grey: #D3D3D3;
    --grey: #818181;
    --dark-grey: #3e3e3e;
    --black: #000;
    --white: #FFF;
  }
*/

  /* Base setup */
  :root {
      font-size: 100%;
  }

  /* Set up a decent box model on the root element */
  html {
      box-sizing: border-box;
  }

  /* Make all elements from the DOM inherit from the parent box-sizing
     Since `*` has a specificity of 0, it does not override the `html` value
     making all elements inheriting from the root box-sizing value
     See: https://css-tricks.com/inheriting-box-sizing-probably-slightly-better-best-practice/ */
  *,
  *::before,
  *::after {
    box-sizing: inherit;
  }

  body {
    font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
    font-size: 1rem;
    line-height: 1.5rem;
  }

  /* Set up the vertical margin for important base block elements. Add any others as required */
  p,
  ul,
  ol,
  div,
  section {
      margin-bottom: 1.5rem;
  }

  .header {
    margin-bottom: 1rem;
  }

</style>
