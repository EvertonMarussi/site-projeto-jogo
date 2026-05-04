<template>
  <div>
    <SiteStruture />
  </div>
</template>

<script>

import SiteStruture from './layouts/SiteStruture.vue';

export default {
  name: 'App',
  components: {
    SiteStruture
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  
}
</style>
