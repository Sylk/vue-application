<template>
  <div id="app">
    <Header/>
    <div class="container" style="display:grid; grid-template-columns:50% 50%">
      <NewDeskCard 
        manufacturer = "Steelcase"
      />
      <DeskCard 
        manufacturer = "Steelcase"
        manufacturerDate = "June 2nd 1945"
        weight = 345
        colorVariation = "Creamy"
        condition = "Aggressively Used"
        price = 430
        shipping = 345
      />
      <DeskCard 
        manufacturer = "Jarvis"
        manufacturerDate = "April 22nd 2016"
        weight = 235
        colorVariation = "Oak"
        condition = "Gently Used"
        price = 1300
        shipping = 45
      />
      <DeskCard 
        manufacturer = "Ikea"
        manufacturerDate = "January 15th 2018"
        weight = 50
        colorVariation = "Teak"
        condition = "Unopened"
        price = 45
        shipping = 25
      />
      <DeskCard 
        manufacturer = "Herman Miller"
        manufacturerDate = "April 22nd 2011"
        weight = 145
        colorVariation = "Space Gray"
        condition = "Unopened"
        price = 780
        shipping = 65
      />
    </div>
  </div>
</template>

<script>
import NewDeskCard from './components/NewDeskCard.vue'
import DeskCard from './components/DeskCard.vue'
import Header from './components/Header.vue'

export default {
  name: 'app',
  components: {
    NewDeskCard,
    DeskCard,
    Header
  }
}
</script>