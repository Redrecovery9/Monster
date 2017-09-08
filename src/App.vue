<template>
  <div id="app">
    <header></header>
    <cards></cards>
    <post></post>
  </div>
</template>

<script>
import Header from './components/Header'
import Cards from './components/Cards'
import Post from './components/Post'

export default {
  name: 'app',
  components: {
    Header,
    Cards,
    Post
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
