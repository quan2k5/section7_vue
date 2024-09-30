<script setup>
import todoItem from './TodoItem.vue'
import {ref} from 'vue'
let str=ref();
const handleMessage=(data)=>{
    str.value=data;
}
</script>
<template>
<div>
    <todo-item @messageSent='handleMessage'></todo-item>
    <div>Id delete:{{str}}</div>
</div> 
</template>
<style scoped></style>
