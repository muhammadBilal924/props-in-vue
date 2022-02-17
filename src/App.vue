<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <h1>Props in vue js </h1>
     <Child v-bind:name="usreName" /> 
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
 import Child from './components/Child.vue'
export default {
  name: 'App',
  components: {
    // HelloWorld,
    Child,

  },
  data(){
    return {users:[
      {name:"Abdullah:Abdullah@test.com"},
      {name: "Numan:Numan@test.com"},
      {name: "Sufyan:Sufyan@test.com"},
      {name: "Zain:Zain@test.com"},
       {name: "Bilal:Bilal@test.com"}
      
    ]}
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
