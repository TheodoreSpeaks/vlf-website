<template>
    <v-app-bar
      app
      color="background"
      dark
      flat
    >
    <v-img alt="Vivian Likes Fruit" contain height="60" width="0" src="../assets/vlf_logo.png"/>
    <v-spacer/>
    <div class="header-links" v-for="(appbar_link, i) in appbar_links" :key="i">
      <v-btn color="black" :href="appbar_link.href" plain>
        {{ appbar_link.name }}
      </v-btn>
    </div>
    </v-app-bar>
</template>

<script>
export default {
  name: 'AppBar',

  data: () => ({
    appbar_links: [
      { name: 'Art', href: '/art' },
      { name: 'Blog', href: '/blog' },
      { name: 'Comics', href: '/comics' },
      { name: 'Projects', href: 'projects' },
      { name: 'About', href: '/about' }
    ],
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
