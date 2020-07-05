<template>
  <div id="app">
    <product-list-one></product-list-one>
    <product-list-two></product-list-two>
  </div>
</template>

<script>
import productOne from './components/product-list-one'
import productTwo from './components/product-list-two'

export default {
  name: 'App',
  data() {
    return {}
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
