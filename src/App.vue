<template>
  <div id="app">
    <toolbar></toolbar>
    <cards></cards>
    <post></post>
  </div>
</template>

<script>
import Toolbar from './components/Toolbar'
import Cards from './components/Cards'
import Post from './components/Post'
const baseURL = 'https://monsters-app.herokuapp.com/api/v1'

export default {
  name: 'app',
  components: {
    Toolbar,
    Cards,
    Post
  },
  async mounted(){
    const data = await fetch(`${baseURL}/monsters`)
    const response = await data.json()

  },
}
</script>

<style>
.toolbar {
  display: flex;
  justify-content: center;
  background-color: #dbd6d6;
  margin-bottom: 1em;
}

</style>
