<template>
</template>

<script>
export default {
  name: 'AppBar',

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
