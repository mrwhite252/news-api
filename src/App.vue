<template>
  <div id="nav">
    <router-link to="/">News Update</router-link> |
    <router-link to="/about">Medal Rankings</router-link>
  </div>
  <router-view />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  color: #2c3e50;
}

#nav {
  padding: 30px;
  text-align: center;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
  transition: 0.2s all ease-out;
}

#nav a.router-link-exact-active {
  color: white;
  background: #42b983;
  padding: 0.5em;
  border-radius: 5px;
}
</style>
