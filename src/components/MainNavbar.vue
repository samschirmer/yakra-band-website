<template>
  <nav class="navbar is-fixed-top is-black" role="navigation" aria-label="main navigation">
    <a role="button" class="navbar-burger" @click="isActive = !isActive" :class="{ 'is-active': isActive }" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>
        
    <div class="navbar-menu" :class="{ 'is-active': isActive }">
        <RouterLink class="navbar-item is-expanded" to="/">home</RouterLink>
        <RouterLink class="navbar-item is-expanded" to="/music">music</RouterLink>
        <a class="navbar-item is-expanded" href="https://yakra.bandcamp.com">store</a>
        <RouterLink class="navbar-item is-expanded" to="/about">about</RouterLink>
        <RouterLink class="navbar-item is-expanded" to="/contact">contact</RouterLink>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'MainNavbar',
  data() {
    return {
      isActive: false,
    };
  },
};
</script>

<style scoped>
  .navbar-item {
    display: flex; 
    justify-content: center; 
    align-items: center;
    width: 100%;
  }

  .navbar-menu {
    background-color: #000 !important;
  }

  .navbar {
    max-width: 100vw;
  }

  .navbar-link.is-active, .navbar-link:focus, .navbar-link:focus-within, .navbar-link:hover, a.navbar-item.is-active, a.navbar-item:focus, a.navbar-item:focus-within, a.navbar-item:hover {
    background-color: #0a0a0a;
    color: #fff;
  }

  a {
    text-decoration: none;
  }
</style>
