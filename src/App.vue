<script setup>
import { reactive } from 'vue';
import Cart from './components/Cart.vue';
import CartComposition from './components/CartComposition.vue';

const articles = reactive([
  {
    id: 1,
    name: 'Artikel 1',
    quantity: 2,
    price: 1.0,
  },
  {
    id: 2,
    name: 'Artikel 2',
    quantity: 3,
    price: 2.0,
  },
]);
</script>

<template>
  <Cart :articles="articles" />
  <CartComposition :articles="articles" />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
