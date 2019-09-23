<template>
  <div class="about">
    <h1>
      Hey You!
    </h1>
    <h2>
      This page was created by Jonny Frey. You can check out the code at <a href="https://github.com/JonnyFrey/waffel-web">github</a>.
    </h2>
  </div>
</template>

<style scoped>
  h1 {
    font-size: 500%;
    color: limegreen;
  }

  h2 {
    font-size: 150%;
    color: limegreen;
  }

  .about {
    position: absolute;
    top: 50%;
    left: 50%;
    -moz-transform: translateX(-50%) translateY(-50%);
    -webkit-transform: translateX(-50%) translateY(-50%);
    transform: translateX(-50%) translateY(-50%);
    margin: 0 -50% 0 0;
  }
</style>
