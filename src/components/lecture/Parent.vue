<script setup>
import Child from './Child.vue'
import {ref} from 'Vue'
let message=ref('hello!')
let age=ref(5)
</script>
<template>
<div>
  <h3>Parrent</h3>
  <child  :propName="message" :age='age'>
    <template #intro >
        <h3>hoc lap trinh vue js</h3>
    </template>
    <p>Gia tri nhan e tu component con:{{item}}</p>
  </child>
</div>
</template>
<style scoped>
</style>
