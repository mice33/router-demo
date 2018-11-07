<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      <a @click="back">go back</a>
    </p>
  </div>
</template>

<script>
export default {
  name: 'h2page',
  data () {
    return {
      msg: 'h2 Page'
    }
  },
  methods: {
    back() {
      this.$router.back();
    }
  }
}
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
