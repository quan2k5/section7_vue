<script setup>
const props=defineProps(["propName","age"]);
console.log('gia tri cua props',props);
</script>

<template>
<div>
  <h3>Child</h3>
  <p>Gia trj nhan ve tu component cha la {{props.propName}}</p>
  <p>Tuoi:{{props.age}}</p>
  <p>noi hien thi cua hoc lap trinh vue js</p>
  <slot :item='data' name="intro" ></slot>
  <p>noi hien thi cua phan tim hieu slot</p>
</div>
</template>

<style scoped>
</style>
