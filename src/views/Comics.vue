<template>
  <v-app>
    <h1>ID: {{ id }}</h1>
    <h1>ID: {{ id }}</h1>
  </v-app>
</template>

<script>
export default {
  name: 'Comics',
  computed: {
    id() {
      return this.$route.params.id || -1
    }
  }

}
</script>

<style>

</style>