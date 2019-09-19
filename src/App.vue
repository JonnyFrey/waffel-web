<template>
  <div id="app">
    <div>
      <Slide id="nav">
        <router-link to="/">
          <b-icon
                  pack="fas"
                  icon="home"
                  size="is-medium"
                  type="is-info">
          </b-icon>
          <div class="icon-name">
            Home
          </div>
        </router-link>
        <router-link to="/about">
          <b-icon
                  pack="fas"
                  icon="info-circle"
                  size="is-medium"
                  type="is-info">
          </b-icon>
          <div class="icon-name">
            About
          </div>
        </router-link>
      </Slide>
    </div>
    <div id="section">
      <router-view/>
    </div>
  </div>
</template>

<script>
  import { Slide } from 'vue-burger-menu';

  export default {
    components: {
      Slide,
    },
  };
</script>

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

  #nav .bm-menu {
    background: #1c1c1c;
  }

  #nav .bm-burger-bars {
    background: limegreen;
  }

  #nav .bm-cross {
    left: -20%;
    top: 20%;
  }

  #nav .icon-name {
    padding-left: 10%;
    padding-top: 1%;
  }

</style>
