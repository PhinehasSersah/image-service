<template>
  <ImageDisplay />
</template>

<script>
import ImageDisplay from './components/ImageDisplay.vue'

export default {
  name: 'App',
  components: {
    ImageDisplay
  }
}
</script>

<style>
* {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
   background: #ecf0f1;
}
</style>
