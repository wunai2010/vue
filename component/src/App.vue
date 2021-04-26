<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <component :is="HelloWorld" @msg="你好"></component>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
	<MESSAGE msg="你好"></MESSAGE>
	<MESSAGE msg="你好"></MESSAGE>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import MESSAGE from './components/h1.vue';

var components1 = {HelloWorld,MESSAGE};
export default {
  name: 'App',
  data:function(){
	return {allComponents:['HelloWorld','MESSAGE']}
  },
  components:components1
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
