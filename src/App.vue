<template>
  <div id="app">
    <Header/>

    <main>
      <Hero/>
      <!-- vv page vv -->
      <foodieJournal/>
    </main>

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'

import foodieJournal from './components/index-comp/foodieJournal.vue'

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    foodieJournal,
  }
}
</script>

<style lang="scss">
@import './assets/style/style.scss';


</style>
