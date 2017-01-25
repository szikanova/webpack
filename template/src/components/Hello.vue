<template>
  <div class="hello">
    <h1>Hello World My Name is sophia!</h1>
    <input v-model="message" placeholder="edit me">
  </div>
</template>

<script>
export default {
  name: 'hello',
  data:{{#unless_eq lintConfig "airbnb"}} {{/unless_eq}}() => {
    return {
      message: 'sophia'
    }{{#if_eq lintConfig "airbnb"}};{{/if_eq}}
  }{{#if_eq lintConfig "airbnb"}},{{/if_eq}}
}{{#if_eq lintConfig "airbnb"}};{{/if_eq}}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
