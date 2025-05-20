<script setup>
import { ref } from 'vue'

const product = ref('Jacket')
</script>

//add a product description ref to your script section.
//displiay the description using an expression in a  p tag.

<template>
  <div class="product-display">
    <div class="product-container">
      <div class="product-info">
        <p>{{product}}</p>
      </div>
    </div>
  </div>
</template>