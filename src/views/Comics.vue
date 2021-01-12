<template>
  <v-app>
    <h1>ID: {{ id }}</h1>
    <h1>ID: {{ id == null }}</h1>
  </v-app>
</template>

<script>
export default {
  name: 'Comics',
  data: () => ({
    // TODO: change to latest comic #
    id: this.$route.params.id || -1
  })

}
</script>

<style>

</style>