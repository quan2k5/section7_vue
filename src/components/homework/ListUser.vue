<script setup>
import FormAddUser from './FormAddUser.vue'
import {ref} from 'vue'
const checkForm=ref(false);
const handleClick=()=>{
    checkForm.value=true;
}
const handleClose=(data)=>{
    checkForm.value=data;
}
</script>
<template>
<div>
    <button v-on:click="handleClick">Add user</button>
    <template v-if="checkForm">
        <form-add-user @messageSent='handleClose'></form-add-user>
    </template>
</div>
</template>
<style scoped></style>