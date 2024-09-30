<template>
  <button :type="type" @click="handleClick">
    <slot></slot>
  </button>
</template>
<script setup>
import { defineProps, defineEmits } from 'vue';
const props = defineProps(['type']);
const emit = defineEmits(['messageSent']);
const handleClick = () => {
  emit('messageSent');
};
</script>
<style scoped>
</style>
