<template>
  <div id="app">
    <app-header @menuSwitched="switchMenu($event)"></app-header>
    <component :is="mode"></component>
  </div>
</template>

<script>
  import Header from './components/Header.vue';
  import Home from './components/Home.vue';
  import Ranking from './components/Ranking.vue';
  import Random from './components/Random.vue';

  export default {
    name: 'app',
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
      appHeader: Header,
      appHome: Home,
      appRanking: Ranking,
      appRandom: Random
    }
  }
</script>

<style>
  #app {
  }
</style>
