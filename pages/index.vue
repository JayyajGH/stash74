<template>
  <div class="wrapper--full-height">
    <header>
			<img src="~/assets/images/logo.svg" class="logo2"/>
  	</header>

    <main class="wrapper" id="wrapper">
      <nav class="nav">
        <ul class="nav__menu">
				  <li class="nav__item nav--home">
            <router-link class="nav__link" to="/">
              <div class="nav__group">
                <span class="nav__text">Home</span>
                <span class="fas fa-home nav__icon"></span>
              </div>
            </router-link>
          </li>
          <li class="nav__item nav--projects">
            <router-link class="nav__link" to="/projects">
              <div class="nav__group">
                <span class="nav__text">Projects</span>
                <span class="fas fa-briefcase nav__icon"></span>
              </div>
            </router-link>
          </li>
          <li class="nav__item nav--about">
            <router-link class="nav__link" to="/about">
              <div class="nav__group">
                <span class="nav__text">About</span>
                <span class="fas fa-book-open nav__icon"></span>
              </div>
            </router-link>
          </li>
          <li class="nav__item nav--contact">
            <router-link class="nav__link" to="/contact">
              <div class="nav__group">
                <span class="nav__text">Contact</span>
                <span class="fas fa-user nav__icon"></span>
              </div>
            </router-link>
          </li>
        </ul>
      </nav>
    </main>
  </div>
</template>

<script>

export default {
}
</script>

<style>
  :root {
    --light-grey: #D3D3D3;
    --grey: #818181;
    --dark-grey: #3e3e3e;
    --black: #000;
    --white: #FFF;
  }

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

  /* Use perfect fourth modular scale */
  body {
    font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
    font-size: 1rem;
    line-height: 1.5rem;
  }

  .heading1 {
    font-size: 2.369rem;
    margin-bottom: 2rem;
  }

  .heading2 {
    font-size: 1.777rem;
    margin-bottom: 1rem;
  }

  .small-text {
    font-size: 0.75rem;
    margin-bottom: 0.5rem;
  }

  .header {
    background-color: var(--white);
    margin-bottom: 1rem;
  }

  .logo2 {
    height: 60px;
    position: absolute;
    transform: translateY(-50%) rotate(90deg);
    top: 50%;
    right: -90px;
  }

  @media (min-width: 800px) {
    .logo2 {
      left: 50%;
      transform: translateX(-50%);
      top: 0;
      right: -120px;
    }
  }

  .nav__menu {
    min-height: 100%;
    display: flex;
    flex-direction: column;
  }

  @media (min-width: 800px) {
    .nav__menu {
      flex-direction: row;
    }
  }

  .nav__item {
      flex: 1;
      display: flex;
      justify-content: center;
      flex-direction: column;
      text-align: center;
  }

  .nav__link {
      text-decoration: none;
      display: flex;
      width: 100%;
      min-height: 100%;
      flex-direction: row;
      align-items: center;
      color: #000;
  }

  .nav__group {
      flex: 1;
      display: flex;
      flex-direction: column;
  }

  .nav__text {
      font-size: 20px;
      padding-bottom: 10px;
  }

  .nav__icon {
      font-size: 5em;
  }

  @media (min-width: 800px) {
    .nav__icon {
      font-size: 7em;
    }
  }

  .fa-home {
    transition: 0.8s;
  }

  .nav__item:hover .fa-home  {
    font-size: 6em;
    transition: 0.8s;
  }

  @media (min-width: 800px) {
    .nav__item:hover .fa-home  {
      font-size: 8em;
    }
  }

  .fa-briefcase {
    transition: 0.8s;
  }

  .nav__item:hover .fa-briefcase {
    font-size: 6em;
    transition: 0.8s;
  }

  @media (min-width: 800px) {
    .nav__item:hover .fa-briefcase  {
        font-size: 8em;
    }
  }

  .fa-book-open {
    transition: 0.8s;
  }

  .nav__item:hover .fa-book-open  {
    font-size: 6em;
    transition: 0.8s;
  }

  @media (min-width: 800px) {
    .nav__item:hover .fa-book-open  {
      font-size: 8em;
    }
  }

  .fa-user {
    transition: 0.8s;
  }

  .nav__item:hover .fa-user  {
    font-size: 6em;
    transition: 0.8s;
  }

  @media (min-width: 800px) {
    .nav__item:hover .fa-user  {
      font-size: 8em;
    }
  }

  .nav--home {
    background-color: rgba(65, 244, 113, 0.7);
    border: 1px solid rgb(65, 244, 113);
  }

  .nav--home:hover {
    background-color: rgb(65, 244, 113);
    transition: 0.8s;
  }

  .nav--projects {
    background-color: rgba(65, 104, 244, 0.7);
    border: 1px solid rgb(65, 104, 244);
  }

  .nav--projects:hover {
    background-color: rgb(65, 104, 244);
    transition: 0.8s;
  }

  .nav--about {
    background-color: rgba(244, 66, 69, 0.7);
    border: 1px solid rgb(244, 66, 69);
  }

  .nav--about:hover {
    background-color: rgb(244, 66, 69);
    transition: 0.8s;
  }

  .nav--contact {
    background-color: rgba(244, 160, 65, 0.7);
    border: 1px solid rgb(244, 160, 65);
  }

  .nav--contact:hover {
    background-color: rgb(244, 160,65);
    transition: 0.8s;
  }

  html,
  body,
  nav,
  main,
  .wrapper--full-height,
  #__nuxt,
  #__layout {
    height: 100%;
  }
</style>
