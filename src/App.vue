<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>

    {{testENV}}
  </nav>
  <router-view/>
</template>

<style lang="scss">
 @import "bootstrap";
</style>

<script>
export default {
  data () {
    return {
      testENV: process.env.VUE_APP_API_KEU
    }
  }
}
</script>
