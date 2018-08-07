<template>
<div>
    <h1 :prop="manufacturer">{{manufacturer}}</h1>
    <ul>
      <li>Manufacture Date: {{manufacturerDate}}</li>
      <li>Weight: {{weight}} lbs</li>
      <li>Color Variation: {{colorVariation}}</li>
      <li>Condition: {{ condition }}</li>
      <li>Price: {{ price }} USD</li>
      <li>Shipping: {{ shipping }} USD</li>
    </ul>
</div>  
</template>

<script>
// import json from "../../json/data.json";

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