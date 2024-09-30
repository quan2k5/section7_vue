<script setup>
import CountChildren from './CountChildren.vue'
import {ref} from 'vue'
const data=false;
const emit=defineEmits(['messageSent'])
const closeForm=()=>{
    emit("messageSent",data);
}
</script>
<template>
<div>
    <div>Form Add user</div>
    <div>
        <label for="">Name</label>
        <input type="text">
    </div>
      <div>
        <label for="">Email</label>
        <input type="text">
    </div>
    <div>
        <label for="">Address</label>
        <input type="text">
    </div>
    <div>
        <button @click="closeForm">Close</button>
    </div>
</div>
</template>
<style scoped></style>
