<template>
  <v-app id="app">
    <v-app-bar
      app
      color="background"
      dark
      flat
    >
      <!-- <h1> Vivian Likes fruit? </h1> -->
    <router-link to="/">
      <img alt="Vivian Likes Fruit" contain height="60" src="@/assets/vlf_logo.png"/>
    </router-link>
    <v-spacer/>
    <v-app-bar-nav-icon v-if="isMobile" @click.stop="drawer = !drawer" color=grey></v-app-bar-nav-icon>
    <div v-else class="header-links" v-for="(appbar_link, i) in appbar_links" :key="i">
      <v-btn color="black" :href="appbar_link.href" plain>
        {{ appbar_link.name }}
      </v-btn>
    </div>
    </v-app-bar>
    <router-view/>
        <v-navigation-drawer
      v-model="drawer"
      absolute
      temporary
      right
    >
      <v-list
        nav
        dense
      >
          <v-list-item v-for="(appbar_link, i) in appbar_links" :key="i">
            <router-link :to="appbar_link.href">
              <v-list-item-title>{{ appbar_link.name }}</v-list-item-title>
            </router-link>
        </v-list-item>
      </v-list>
        </v-navigation-drawer>
  </v-app>
</template>
<script>

export default {
  name: 'AppMain',
  data: () => ({
    drawer: false,
    appbar_links: [
      { name: 'Art', href: '/art' },
      { name: 'Blog', href: '/blog' },
      { name: 'Comics', href: '/comics' },
      { name: 'Projects', href: 'projects' },
      { name: 'About', href: '/about' }
    ],
  }),
  computed: {
    isMobile() {
      return this.$vuetify.breakpoint.xs || this.$vuetify.breakpoint.sm
    }
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
.header-links {
  font-size: 24px;
}

a:link, a:visited {
  text-decoration: none;
  color: black;
}


</style>
