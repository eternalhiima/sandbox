<template>
  <div id="header">
    <link href="https://fonts.googleapis.com/css?family=Gamja+Flower" rel="stylesheet">
    <b-navbar toggleable="md" type="dark" variant="info">

      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>

      <b-navbar-brand class="b-navbar-brand" @click="switchMenu('app-home')">hiima</b-navbar-brand>

      <b-collapse is-nav id="nav_collapse">

        <b-navbar-nav>
          <b-nav-item @click="switchMenu('app-ranking')">Ranking</b-nav-item>
          <b-nav-item @click="switchMenu('app-random')">Random</b-nav-item>
          <b-nav-item href="#" disabled>Login</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">

          <b-nav-form>
            <b-form-input size="sm" class="mr-sm-2" type="text" placeholder="Search"/>
            <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
          </b-nav-form>

          <!--dropdown-->
          <!--<b-nav-item-dropdown text="Lang" right>-->
            <!--<b-dropdown-item href="#">EN</b-dropdown-item>-->
            <!--<b-dropdown-item href="#">ES</b-dropdown-item>-->
            <!--<b-dropdown-item href="#">RU</b-dropdown-item>-->
            <!--<b-dropdown-item href="#">FA</b-dropdown-item>-->
          <!--</b-nav-item-dropdown>-->

          <!--when logged in-->
          <!--<b-nav-item-dropdown right>-->
            <!-- Using button-content slot -->
            <!--<template slot="button-content">-->
              <!--<em>User</em>-->
            <!--</template>-->
            <!--<b-dropdown-item href="#">Profile</b-dropdown-item>-->
            <!--<b-dropdown-item href="#">Signout</b-dropdown-item>-->
          <!--</b-nav-item-dropdown>-->

        </b-navbar-nav>

      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
  export default {
    name: 'app-header',
    data () {
      return {
      }
    },
    methods: {
      switchMenu(menu){
        this.$emit('menuSwitched',menu);
      }
    }
  }
</script>

<style>
  .b-navbar-brand {
    font-family: 'Gamja Flower', cursive;
    font-size: 250%;
  }
</style>
