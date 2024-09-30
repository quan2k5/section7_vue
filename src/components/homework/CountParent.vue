<script setup>
import CountChildren from './CountChildren.vue'
import {ref} from 'vue'
let count=ref(0);
const handleMessage=()=>{
    count.value+=1;
}
</script>
<template>
<div>
    <count-children @messageSent="handleMessage"></count-children>
    <div>Count:{{count}}</div>
</div>
</template>
<style scoped></style>
