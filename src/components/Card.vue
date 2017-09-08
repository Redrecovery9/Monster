<template>
  <div>
      <div class="container">
        <h2 class="title">Monster Name</h2>
        <img src="https://lorempixel.com/600/300/food/5/">

      </div>
  </div>
</template>

<script>
export default {
  name: 'card',
  data () {
    return {

    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.container{
  border: 1px solid #CCC;
  padding: 20px;
  background-image: url(http://www.ericwallen.tech/src/app/fire.gif);
  max-width: 400px;
  overflow: hidden;
}



.container img{
  width: 100%
}

.title{
  text-align: center;
  color: #FFF;
}

</style>
