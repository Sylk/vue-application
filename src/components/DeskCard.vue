<template>
<div>
    <h1>{{desk.manufacturer}}</h1>
    <ul>
      <li>Manufacture Date: {{desk.manufacturerDate}}</li>
      <li>Weight: {{desk.weight}} lbs</li>
      <li>Color Variation: {{desk.colorVariation}}</li>
      <li>Condition: {{desk.condition}}</li>
      <li>Price: {{desk.price}} USD</li>
      <li>Shipping: {{desk.shipping}} USD</li>
    </ul>
</div>  
</template>

<script>

export default {
  props: ['desk']
};
</script>