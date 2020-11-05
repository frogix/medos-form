<template>
  <div id="app">
    <InputElement name="someName"/>
  </div>
</template>

<script>
import InputElement from './components/InputElement.vue'

export default {
  name: 'App',
  components: {
    InputElement
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
