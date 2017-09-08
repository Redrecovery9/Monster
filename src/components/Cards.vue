<template>
  <div class="cards">
    <Card v-for="monster in monsters" :monster='monster' key=""></Card>
  </div>
</template>

<script>
import Card from './Card'

export default {
  name: 'Cards',
  props: ['monsters'],
  components: {
    Card
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
