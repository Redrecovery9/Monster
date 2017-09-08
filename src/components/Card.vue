<template>
  <div class="cards">
    <b-container>
        <b-row>
          <b-col>
            <div>
              <b-card title="Hello"
                      img-src="https://lorempixel.com/600/300/food/5/"
                      img-alt="Image"
                      img-top
                      tag="article"
                      style="max-width: 20rem;"
                      class="mb-2">
                <p class="card-text">
                  Some quick example text to build on the card title and make up the bulk of the card's content.
                </p>
                <b-button href="#" variant="primary">Go somewhere</b-button>
              </b-card>
            </div>
          </b-col>
        </b-row>
    </b-container>
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

</style>
