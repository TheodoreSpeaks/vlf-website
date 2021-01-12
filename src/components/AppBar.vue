<template>
    <v-app-bar
      app
      color="background"
      dark
      flat
    >
      <!-- <h1> Vivian Likes fruit? </h1> -->
    <router-link to="/">
      <img alt="Vivian Likes Fruit" contain height="60" src="../assets/vlf_logo.png"/>
    </router-link>
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
.header-links {
  font-size: 24px;
}

a:link, a:visited {
  text-decoration: none;
  color: black;
}

</style>
