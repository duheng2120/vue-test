<!--  -->
<template>
  <div class="person">
    <h2>姓名：{{ name }}</h2>
    <h2>年龄：{{ age }}</h2>
    <button @click="showTels">查看联系方式</button>
  </div>
</template>

<script setup lang="ts">
  import {ref } from 'vue';

  let name = ref('张三')
  let age = ref(18)
  let tel = '12399999999'

  function changeName() {
    name.value = 'zhangsan'
  }

  function showTels(){
    alert(tel);
  }
</script>

<style scoped>
.person{
  background-color: rgb(154, 45, 87);
  box-shadow: 0 0 10px;
  border-radius: 10px;
  padding: 20px;
}
</style>
