<template>
  <div id="app">
    <Header/>
    <div class="container" style="display:grid; grid-template-columns:50% 50%">
      <NewDeskCard/>
      <DeskCard v-for='(desk,index) in inventory' :key='index' :desk='desk'/>
    </div>
  </div>
</template>

<script>
import NewDeskCard from './components/NewDeskCard.vue'
import DeskCard from './components/DeskCard.vue'
import Header from './components/Header.vue'
import data from '../json/data.json'
import jQuery from 'jquery'
import popper from 'popper.js'
import Bootstrap from 'bootstrap'

export default {
  name: 'app',
  components: {
    NewDeskCard,
    DeskCard,
    Header
  },
  data () {
    return {
      inventory: data.inventory
    }
  }
}
</script>