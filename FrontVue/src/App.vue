<template>
  <HomeView/>
</template>

<script>
import HomeView from './Views/HomeView.vue'

export default {
  name:'App',
  components: {
    HomeView,
  }
}
</script>

<style>

#app{
  padding: 0;
  margin: 0;
}
body{
    height: 100%;
    overflow-x: hidden;
}
</style>

