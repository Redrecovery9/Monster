<template>
  <div>

    <div v-if='!monster.scary' class="container" style="background: url(http://dribbble.s3.amazonaws.com/users/41276/screenshots/332290/animated-rainbow.gif)">
      <h2 class="title black">{{monster.name}}</h2>
      <img :src="monster.image">
    </div>
    <div v-else='monster.scary' class="container" style="background: url(https://rasica.files.wordpress.com/2014/04/fire-5.gif)">
      <h2 class="title white">{{monster.name}}</h2>
      <img :src="monster.image">
    </div>
      <div class="desc-container">
        <p>{{monster.description}}</p>
      </div>
  </div>
</template>

<script>
export default {
  name: 'card',
  props: ['monster'],
  data () {
    return {

    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.container{
  padding: 20px;
  background:  no-repeat center center fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  max-width: 800px;
  margin: 0 auto;

}

.desc-container{
  padding: 40px;
  max-width: 800px;
  margin: 0 auto;
  margin-bottom: 40px;
  border: 1px solid #CCC;
}

.container img{
  width: 100%
}

.black{
  text-align: center;
  color: #050505;
  font-weight: bolder;
}

.white{
  text-align: center;
  color: #FFF;
  font-weight: bolder;
}

</style>
