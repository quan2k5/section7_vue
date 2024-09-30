<script setup>
import {ref} from'vue';
import Header from './components/lecture/Header.vue'
import ParentComponent from './components/homework/ParentComponent.vue'
import ProductParent from './components/homework/ProductParent.vue'
import CountParent from './components/homework/CountParent.vue'
import TodoApp from './components/homework/TodoApp.vue'
import Modal1 from './components/homework/Modal.vue'
import Card1 from './components/homework/Card.vue'
import MessageParrent1 from './components/homework/MessageParent.vue'
import ListUser from './components/homework/ListUser.vue'
import BaseButton from './components/homework/BaseButton.vue'
import BaseInput from './components/homework/BaseInput.vue'
// ham nhan gia tri tu component con
const handleMessage=(data)=>{
  console.log('gia tri nhan ve',data);
}
const checkModal=ref(true)
const handleClose=()=>{
  checkModal.value=false;
}
const modelValue=ref('');
const type=ref('text');
const placeHolder=ref("nhap 1 chuoi")
const typeButton=ref('submit');
const handleChange=(data)=>{
  modelValue.value=data;
}
const handleClick1=()=>{
  console.log('run11111111');
  
}
</script>
<template>
<div>
  <h3>Session 07</h3>
  <ul>
    <li>Props</li>
    <li>slots</li>
    <li>emit</li>
  </ul>
  <parent></parent>
  <Header @messageSent="handleMessage"></Header>
  <p>Bai 1</p>
  <parent-component></parent-component>
  <p>Bai 2</p>
  <product-parent></product-parent>
  <p>Bai 3</p>
  <count-parent></count-parent>
  <p>Bai 4</p>
  <todo-app></todo-app>
  <p>Bai 5</p>
  <Modal1>
    <template v-if="checkModal">
      <h4>Thong bao tu he thong</h4>
      <div>Day la noi dung cua modal.ban co the dong model bang cach nhan nut close</div>
      <button @click="handleClose">Close</button>
    </template>
  </Modal1>
  <p>Bai 6</p>
  <card1>
    <template #header>
      <span>Thong tin san pham</span>
    </template>
    <template #body>
      <span>Day la mo ta ngan gon ve san pham nay.San pham co cac tinh nang noi bat va gia ca hop ly</span>
    </template>
    <template #footer>
      <button>Xem chi tiet</button>
    </template>
  </card1>
  <p>Bai 7</p>
  <MessageParrent1></MessageParrent1>
  <p>Bai 8</p>
  <list-user></list-user>
  <p>Bai 9</p>
  <base-button @messageSent='handleClick1' :type='typeButton' >
      <span>{{typeButton}}</span>
  </base-button>
  <p>Bai 10</p>
  <base-input @messageSent="handleChange" :type="type" :modelValue='modelValue' :placeHolder="placeHolder">
        <p>Gia tri trong o input la {{modelValue}}</p>
  </base-input>
</div>
</template>
<style scoped>
</style>
