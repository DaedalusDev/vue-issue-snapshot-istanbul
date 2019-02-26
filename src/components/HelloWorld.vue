<template>
  <div class="hello">
    <nested-component :fn-value="v => v.value"/>
  </div>
</template>

<script>
import NestedComponent from './NestedComponent'

export default {
  name: 'HelloWorld',
  components: { NestedComponent },
  props: {
    msg: String
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
