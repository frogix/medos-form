<template>
  <div id="app">
    <InputElement
        name="someName"
        type="text"
        label="What is your day?"
        validation="required|email"
        validation-name="Some name"
        placeholder="Type something here..."
        v-model="variable"
    />
  </div>
</template>

<script>
import InputElement from './components/InputElement.vue'

export default {
  name: 'App',
  components: {
    InputElement
  },
  data () {
    return { variable: '' }
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
