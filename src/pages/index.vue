<template>
  <div class="wrapper--full-height">
    <header>
			<img src="~/assets/images/logo.svg" class="logo" alt="Stash74 company logo"/>
  	</header>

    <main class="wrapper" id="wrapper">
      <nav class="nav">
        <ul class="nav__menu">
          <nav-link name="Home" url="/" icon="fa-home" item="nav--home"></nav-link>
          <nav-link name="Projects" url="/page-projects" icon="fa-briefcase" item="nav--projects"></nav-link>
          <nav-link name="About" url="/page-about" icon="fa-book-open" item="nav--about"></nav-link>
          <nav-link name="Contact" url="/page-contact" icon="fa-user" item="nav--contact"></nav-link>
        </ul>
      </nav>
    </main>
  </div>
</template>

<script>
  import NavLink from '@/components/nav-link/nav-link.vue';

  export default {
    components: { NavLink }
  };
</script>

<style scoped lang="scss">
  .logo {
    height: 60px;
    position: absolute;
    transform: translateY(-50%) rotate(90deg);
    top: 50%;
    right: -90px;
  }

  @media (min-width: 800px) {
    .logo {
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

  nav,
  main,
  .wrapper--full-height {
    height: 100%;
  }
</style>

<style>
  html,
  body,
  #__nuxt,
  #__layout {
    height: 100%;
  }
</style>
