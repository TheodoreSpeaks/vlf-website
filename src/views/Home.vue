<template>
  <v-app>
    <ComicView/>
  </v-app>
</template>

<script>
// @ is an alias to /src
import ComicView from '@/components/ComicView.vue'

export default {
  name: 'Home',
  components: {
    ComicView,
  }
}
</script>
