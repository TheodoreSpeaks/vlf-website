<template>
  <v-app>
    <AppBar/>
    <ComicView/>
  </v-app>
</template>

<script>
// @ is an alias to /src
import AppBar from '@/components/AppBar.vue'
import ComicView from '@/components/ComicView.vue'

export default {
  name: 'Home',
  components: {
    AppBar,
    ComicView,
  }
}
</script>
