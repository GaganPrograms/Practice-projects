<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/cart">Cart</router-link>
  </nav>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
  border-radius: 10px;
  background: #e0e0e0;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #ffffff;
  background: #4658e4;
  padding: 15px;
  border-radius: 30px;
}
</style>
