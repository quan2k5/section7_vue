<script setup>
import ProductChildren from './ProductChildren.vue'
let id=1;
let nameProduct='buoi ba roi';
let price=12000

</script>
<template>
<div>
    <product-children :id="id" :nameProduct="nameProduct" :price="price"></product-children>
</div>
</template>
<style scoped>
</style>
