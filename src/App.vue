<template>
  <div id="app">
    <Header :pages="pageList"/>

    <main>
      <Hero/>
      <!-- vv page vv -->
      <foodieJournal/>
      <popularRecipes/>
      <culinaryCollection/>
      <farmToTable/>
    </main>

    <Footer :pages="pageList"/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Footer from './components/Footer.vue'

import foodieJournal from './components/index-comp/foodieJournal.vue'
import popularRecipes from './components/index-comp/popularRecipes.vue'
import culinaryCollection from './components/index-comp/culinaryCollection.vue'
import farmToTable from './components/index-comp/farmToTable.vue'

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    foodieJournal,
    popularRecipes,
    culinaryCollection,
    farmToTable,
    Footer,
  },
  data(){
    return{
      pageList:[
        {
          name: 'Home',
          url: '#',
          current: true,
        },
        {
          name: 'Recipes',
          url: '#',
          current: false,
        },
        {
          name: 'Places',
          url: '#',
          current: false,
        },
        {
          name: 'Blog',
          url: '#',
          current: false,
        },
        {
          name: 'About',
          url: '#',
          current: false,
        },
        {
          name: 'Contact',
          url: '#',
          current: false,
        },
      ],
    }
  }
}
</script>

<style lang="scss">
@import './assets/style/style.scss';


</style>
