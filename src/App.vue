<template>
  <v-app>
    <AppBar/>
    <v-main>
      <ComicView/>
    </v-main>
  </v-app>
</template>

<script>
import AppBar from './components/AppBar';
import ComicView from './components/ComicView.vue';

export default {
  name: 'App',

  components: {
    AppBar,
    ComicView,
  },

  data: () => ({
  }),
};
</script>

<style lang="css">
@import url(https://fonts.googleapis.com/css?family=Quicksand);
.header-links {
  font-size: 24px;
  font-family: 'Quicksand';
}

</style>
