<template>
  <li :class="['nav__item', item]">
    <router-link class="nav__link" :to="url">
      <div class="nav__group">
        <span class="nav__text">{{name}}</span>
        <span :class="['fas nav__icon', icon]"></span>
      </div>
    </router-link>
  </li>
</template>

<script>
  export default {
    name: 'NavLink',
    props: {
      name: {
        type: String,
        required: true
      },
      icon: {
        type: String,
        required: true
      },
      url: {
        type: String,
        required: true
      },
      item: {
        type: String,
        required: true
      }
    }
  };
</script>

<style scoped lang="scss">
  .nav--home {
    background-color: rgba(65, 244, 113, 0.7);
    border: 1px solid rgb(65, 244, 113);
  }

  .nav--home:hover {
    background-color: rgb(65, 244, 113);
  }

  .nav--projects {
    background-color: rgba(65, 104, 244, 0.7);
    border: 1px solid rgb(65, 104, 244);
  }

  .nav--projects:hover {
    background-color: rgb(65, 104, 244);
  }

  .nav--about {
    background-color: rgba(244, 66, 69, 0.7);
    border: 1px solid rgb(244, 66, 69);
  }

  .nav--about:hover {
    background-color: rgb(244, 66, 69);
  }

  .nav--contact {
    background-color: rgba(244, 160, 65, 0.7);
    border: 1px solid rgb(244, 160, 65);
  }

  .nav--contact:hover {
    background-color: rgb(244, 160,65);
  }

  .nav__item {
      flex: 1;
      display: flex;
      justify-content: center;
      flex-direction: column;
      text-align: center;
      transition: 0.8s;
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
      font-weight: 700;
      padding-bottom: 10px;
  }

  .nav__icon {
      font-size: 5em;
      transition: 0.8s;
  }

  @media (min-width: 800px) {
    .nav__icon {
      font-size: 7em;
    }
  }

  .nav__item:hover .nav__icon  {
    font-size: 6em;
    transition: 0.8s;
  }

  @media (min-width: 800px) {
    .nav__item:hover .nav__icon  {
      font-size: 8em;
    }
  }
  
</style>
