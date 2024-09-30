<script setup>
const emit=defineEmits(['messageSent'])
let id=1;
const handleDelete=()=>{
   emit("messageSent",id);
}
</script>
<template>
<div>
    <button @click="handleDelete">Delete</button>
</div>
</template>
<style scoped></style>
