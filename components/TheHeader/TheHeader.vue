<template>
  <header class="main-header">
    <nav class="main-nav">
      <ul class="nav-links">
        <nuxt-link to="/" tag="li" class="nav-link"><a>Home</a></nuxt-link>
        <nuxt-link to="/blog" tag="li" class="nav-link"><a>Blog</a></nuxt-link>
        <nuxt-link to="/contact" tag="li" class="nav-link"><a>Contact</a></nuxt-link>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
.main-header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: #022d30;
  height: 4.5rem;
}

.main-nav {
  height: 100%;
}

.nav-links {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
}

.nav-link {
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0 1rem;
  padding: 0.3rem;
}

.nav-link a{
  display: block;
  text-decoration: none;
  color: white;
}

.nav-link a:hover, .nav-link a:active, nav-link.nuxt-link-exact-active {
  color: #06c4d1;
}
</style>