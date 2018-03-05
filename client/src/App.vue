<template>
  <div id="app">
    <navigation></navigation>
  </div>
</template>

<script>
  import Home from './components/home/home.vue'
  import Navigation from './components/nav/navigation.vue'

  export default {
    components: {
      Home, Navigation
    }
  }
</script>

<style>
  #app {
    position: absolute;
    width: 100%;
    height: 100%;
    left: 0px;
    top: 0px;
  }
</style>
