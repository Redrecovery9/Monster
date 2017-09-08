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
const baseURL = 'https://monsters-app.herokuapp.com/api/v1'

export default {
  name: 'app',
  components: {
    Header,
    Cards,
    Post
  },
  async mounted(){
    const data = await fetch(`${baseURL}/monsters`)
    const response = await data.json()
    
    })
  },
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
h1 {
  background: black;
}
</style>
