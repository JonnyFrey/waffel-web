<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <div id="section">
      <router-view/>
    </div>
  </div>
</template>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    background: #2f3f3f;
    height: 100vw;
  }
  #nav {
    padding: 30px;
  }

  #nav a {
    font-weight: bold;
    color: #502b2f;
  }

  #nav a.router-link-exact-active {
    color: #42b983;
  }
</style>
