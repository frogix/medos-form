<template>
  <div class="form-control">
    <label v-bind:for="name">{{ label }}</label>
    <input
      v-model="inputText"
      v-bind:type="type || 'text'"
      v-bind:placeholder="placeholder"
      v-bind:name="name"
    >
    <h3>You typed: {{inputText.split('').reverse().join('')}}</h3>
  </div>
</template>

<script>
export default {
  name: 'FormControl',
  props: {
    label: String,
    placeholder: String,
    type: String,
    name: String
  },
  data () {
    return { inputText: '' }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
input {
  text-align: left;
}
label {
  font-size: 0.8rem;
  display: block;
  text-align: left;
}
</style>
