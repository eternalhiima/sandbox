<template>
  <div id="ranking">
    <h1>ranking</h1>
    <app-topic-card-board></app-topic-card-board>
  </div>
</template>

<script>
  import TopicCardBoard from '../components/TopicCardBoard.vue';

  export default {
    name: 'app-ranking',
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
