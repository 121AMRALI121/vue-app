<template>
  <div id="app">
    <Test v-for = "obj in objs" :key = "obj.id" :name = "obj.name"/>
  </div>
</template>

<script>

import Test from './components/Test.vue';
import datajs from './components/data.json';
export default {
  name: 'App',
  data(){
    return{
      objs:datajs.items
    }
  },
  components: {
    Test
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
