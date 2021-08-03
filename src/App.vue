<template>
  <div id="app">
    <h2>{{hello}}</h2>
    <h2>{{count}}</h2>
    <button @click="count++">+</button>
    <button @click="count--">-</button>
    <hello-vuex :counter="count"></hello-vuex>
  </div>
</template>

<script>
import helloVuex from './components/helloVuex.vue';
export default {
  name: 'App',
 components:{
    helloVuex
 },
  data(){
    return{
      hello:'我是helloword',
      count:0,
    }
  }
}
</script>

<style>

</style>
