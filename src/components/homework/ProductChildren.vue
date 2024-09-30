<script setup>
const props=defineProps(["id","nameProduct","price"]);
</script>
<template>
<div>
  <div>
    <div>id:{{props.id}}</div>
    <div>Ten san pham:{{props.nameProduct}}</div>
      <div>gia:{{props.price}}</div>
  </div>
</div>
</template>

<style scoped>
</style>
