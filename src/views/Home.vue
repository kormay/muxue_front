<template>
  <div id="home">
    <!--<menu-title></menu-title>-->
    <nav-menu></nav-menu>
    <router-view></router-view>
  </div>
</template>

<style>
  body {
    background: lightpink;
    background-size: 100% auto;
  }
</style>

<script>
  import NavMenu from "./NavMenu"
  export default {
    data () {
      return {}
    },
    components: {
      NavMenu
    }
  }
</script>
