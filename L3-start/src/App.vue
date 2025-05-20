
<script setup>
import { ref } from 'vue'
import socksgreenImage from './assets/images/socks_green.jpeg'

const product = ref('Socks')
const image = ref(socksgreenImage)
const myUrl = ref('https://example.com')

</script>

//add a Url ref to your script section.
//use v-bind to bind the url to the anchor tag href attribute.

<template>
  <div class="nar-bar"></div>
  <div class="product-display">
    <div class="product-container">
      <div class="product-image">
        <!-- image goes here -->
          <img v-bind:src="image"/>
      </div>
    
      <div class="product-info">
        <h1>{{ product }}</h1>
      </div>
        <div>
        <a v-bind:href="myUrl"></a>
      </div>
    </div>
  </div>
</template>