<template>
  <TheHeader />
  <router-view></router-view>
  <TheFooter />
</template>

<script>
import TheHeader from './components/layout/TheHeader.vue'
import TheFooter from './components/layout/TheFooter.vue'
export default {
  components: {
    TheHeader, TheFooter
  }
}
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap");

* {
  box-sizing: border-box;
}

html {
  font-family: "Roboto", sans-serif;
}

body {
  margin: 0;
  background-color: #300322;
  color: #fff;
}
</style>