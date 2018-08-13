<template>
  <div id="app">
    <Header/>
    <div class="container" style="display:grid; grid-template-columns:50% 50%">
      <NewDeskCard/>
      <DeskCard 
        v-for="item in inventory"
        :key="item.id"
        manufacturer = {{item.manufacturer}}
        manufacturerDate = {{item.manufacturerDate}}
        weight = {{item.weight}}
        colorVariation = {{item.colorVariation}}
        condition = {{item.condition}}
        price = {{item.price}}
        shipping = {{item.shipping}}
      />
    </div>
  </div>
</template>

<script>
import NewDeskCard from './components/NewDeskCard.vue'
import DeskCard from './components/DeskCard.vue'
import Header from './components/Header.vue'
import data from '../json/data.json';

export default {
  name: 'app',
  components: {
    NewDeskCard,
    DeskCard,
    Header
  },
  data () {
    return {
      inventory: data
    }
  }
}
</script>