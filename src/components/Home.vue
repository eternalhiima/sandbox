<template>
  <div id="home">
    <h1>home</h1>
    <app-topic-card-board></app-topic-card-board>
  </div>
</template>

<script>
  import TopicCardBoard from '../components/TopicCardBoard.vue';

  export default {
    name: 'app-home',
    data () {
      return {
        mode: 'app-home'
      }
    },
    methods: {
      switchMenu(menu) {
        this.mode = menu;
      }
    },
    components: {
      appTopicCardBoard: TopicCardBoard
    }
  }
</script>

<style>
</style>
