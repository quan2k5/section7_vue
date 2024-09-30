<script setup>
const emit=defineEmits(['messageSent'])
const handleClick=()=>{
   emit("sendMessage");
}
</script>
<template>
<div>
    <button @click="handleClick">sendMessage</button>
</div>
</template>
<style scoped></style>
