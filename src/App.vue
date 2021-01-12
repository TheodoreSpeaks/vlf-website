<template>
  <v-app id="app">
    <div id="nav">
      <AppBar/>
    </div>
    <router-view/>
  </v-app>
</template>
<script>

import AppBar from '@/components/AppBar.vue'
export default {
  name: 'AppMain',
  components: {
    AppBar,
  }
}
</script>

<style lang="scss">
@import url(https://fonts.googleapis.com/css?family=Quicksand);
#app {
  font-family: 'Quicksand', Helvetica, Arial, sans-serif;
  // -webkit-font-smoothing: antialiased;
  // -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  // color: #2c3e50;
}

</style>
