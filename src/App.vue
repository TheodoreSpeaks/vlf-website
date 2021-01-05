<template>
  <v-app>
    <AppBar/>
    <v-main>
      <HelloWorld/>
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';
import AppBar from './components/AppBar';

export default {
  name: 'App',

  components: {
    HelloWorld,
    AppBar,
  },

  data: () => ({
  }),
};
</script>

<style lang="css" scoped>
@import url(https://fonts.googleapis.com/css?family=Quicksand);
.header-links {
  font-size: 24px;
  font-family: 'Quicksand';
}

a:link, a:visited {
  text-decoration: none;
  color: black;
}

</style>
