<template>
  <div id="topic-card-board">
    <div v-for="i in 10">
      <b-card overlay
              img-src="https://picsum.photos/900/250/?image=36"
              img-alt="Card Image"
              text-variant="white"
              title="Image Overlay"
              sub-title="Subtitle">
        <p class="card-text">
          Some quick example text to build on the card and make
          up the bulk of the card's content.
        </p>
        {{ i }}
      </b-card>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'topic-card-board',
    data () {
      return {
      }
    }
  }
</script>

<style>
</style>
