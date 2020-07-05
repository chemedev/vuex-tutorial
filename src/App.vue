<template>
  <div id="app">
    <product-list-one :products="products"></product-list-one>
    <product-list-two :products="products"></product-list-two>
  </div>
</template>

<script>
import productOne from './components/product-list-one'
import productTwo from './components/product-list-two'

export default {
  name: 'App',
  data() {
    return {
      products: [
        { name: 'Banana Skin', price: 20 },
        { name: 'Shiny  Stars', price: 40 },
        { name: 'Green Shells', price: 60 },
        { name: 'Red Shells', price: 80 }
      ]
    }
  },
  components: {
    'product-list-one': productOne,
    'product-list-two': productTwo
  }
}
</script>

<style>
body {
  font-family: Nunito;
  color: #555;
}
</style>
