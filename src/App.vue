
<template>
  <div class="app">
     hello
  </div>
  <Person></Person>
</template>

<script lang="ts">

import Person from './components/Person.vue';

export default{
  name: 'App',  //组件名
  components:{Person}
}
</script>


<style scoped>
.app{
  color: red;
  background-color: #ddd;
  box-shadow: 0 0 10px;
  border-radius: 20px;
  padding: 30px;
}
</style>
