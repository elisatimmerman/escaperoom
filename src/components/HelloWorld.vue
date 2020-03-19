<template>
  <div class="Casussen">
    <h1>Casussen</h1>

    <div v-for="(item, index) in cases" v-bind:key="index">
      <p>{{ item.summary }}</p>
      <p>{{ item.description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data: function () {
  return {
    cases: [{
      'summary':'CVA',
      'description':'Harry heeft problemen met plassen'
    }]
  }
}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
