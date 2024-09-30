<script setup>
const props=defineProps(["type","placeHolder","modelValue"]);
const emit=defineEmits(['messageSent'])
const handleInput=()=>{
   emit("messageSent",event.target.value);
}
</script>
<template>
<div>
   <input @input="handleInput" :type="props.type" :placeholder="placeHolder" :value="modelValue">
   <slot></slot>
</div>
</template>
<style scoped></style>