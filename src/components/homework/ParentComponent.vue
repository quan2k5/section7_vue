<script setup>
import childComponent from './ChildComponent.vue'
let str='Rikkei academy';

</script>
<template>
<div>
    <p>Parent component:{{str}}</p>
    <child-component :propName="str"></child-component>
</div>
</template>
<style scoped>
</style>
