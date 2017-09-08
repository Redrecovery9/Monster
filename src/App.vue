<template>
  <div id="app">
    <toolbar></toolbar>
    <cards :monsters='monsters'></cards>
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
  data() {
    return {
      monsters: []
    }
  },
  async mounted(){
    const data = await fetch(`${baseURL}/monsters`)
    const response = await data.json()
    this.monsters = response.monsters.map(monster => monster)
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
