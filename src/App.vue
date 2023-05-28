<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <sender-component msg="Welcome to Your Vue.js App"/>
  <receiver-component msg="Welcome to Your Vue.js App"/>
</template>

<script>
import SenderComponent from './components/SenderComponent'
import  ReceiverComponent from './components/ReceiverComponent'
export default {
  name: 'App',
  components: {
    SenderComponent,
    ReceiverComponent
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
