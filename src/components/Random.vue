<template>
  <div id="random">
    <h1>random</h1>
    <app-topic-card-board></app-topic-card-board>
  </div>
</template>

<script>
  import TopicCardBoard from '../components/TopicCardBoard.vue';

  export default {
    name: 'app-random',
    data () {
      return {
      }
    },
    components: {
      appTopicCardBoard: TopicCardBoard
    }
  }
</script>

<style>
</style>
