<script setup>
const data='k23_ptit'
const emit=defineEmits(['messageSent'])
const handleClick=()=>{
   emit("messageSent",data);
}
</script>
<template>
<div>
    <h1>K23</h1>
    <button @click="handleClick">an</button>
</div>
</template>
<style scoped></style>
