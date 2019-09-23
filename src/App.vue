<template>
  <div id="app">
    <home-menu-bar/>
    <div id="section">
      <router-view/>
    </div>
  </div>
</template>

<script>
  import HomeMenuBar from '@/components/HomeMenuBar';

  export default {
    name: 'App',
    components: {
      HomeMenuBar,
    },
  };
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    height: 100vh;
  }

  html {
    background-color: #2f3f3f !important;
  }

</style>
