<script setup>
import messageChildren from './MessageChildren.vue'
import {ref} from 'vue'
let count=ref(0);
const handleMessage=()=>{
    alert('welcom to rikkei education')
}
</script>
<template>
<div>
    <message-children @sendMessage="handleMessage"></message-children>
</div>
</template>
<style scoped></style>
