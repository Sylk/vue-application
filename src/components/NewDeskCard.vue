<template>
<div>
    <h1>Manufacturer: <input type="text" :prop="manufacturer"></h1>
    <ul>
      <li>Manufacture Date: <input type="text" :prop="manufacturerDate"/></li>
      <li>Weight: <input type="text" :prop="weight"></li>
      <li>Color Variation: <input type="text" :prop="colorVariation"></li>
      <li>Condition: <input type="text" :prop="condition"></li>
      <li>Price: <input type="text" :prop="price"></li>
      <li>Shipping: <input type="text" :prop="shipping"></li>
    </ul>
    <!-- <button v-on:click="appendItem">Submit</button> -->
</div>  
</template>

<script>

export default {
  props: {
    manufacturer: String,
    manufacturerDate: String,
    weight: String,
    colorVariation: String,
    top: String,
    medium: String,
    bottom: String,
    condition: String,
    price: String,
    shipping: String
  }
};
</script>