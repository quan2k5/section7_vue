<script setup>
const emit=defineEmits(['messageSent'])
const handleClick=()=>{
   emit("messageSent");
}
</script>
<template>
<div>
    <button @click="handleClick">Increament</button>
</div>
</template>
<style scoped></style>
