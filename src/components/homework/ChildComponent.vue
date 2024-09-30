<script setup>
const props=defineProps(["propName"]);
</script>
<template>
<div>
  <div>Children componkent:{{props.propName}}</div>
</div>
</template>

<style scoped>
</style>
