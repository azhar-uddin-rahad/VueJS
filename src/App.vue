<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <HomePage/>
  <h1>Vew Event handler</h1>
  <BasicEvent></BasicEvent>
  <MakeInputForms></MakeInputForms>
  <ToggleButton></ToggleButton>
  <ChildComponents></ChildComponents>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import HomePage from './components/HomePage.vue'
import BasicEvent from './components/BasicEvent'
import MakeInputForms from './components/MakeInputForms'
import ToggleButton from './components/ToggleButton'
import ChildComponents from './components/ChildComponents'
export default {
  name: 'App',
  components: {
    HelloWorld,
    HomePage,
    BasicEvent,
    MakeInputForms,
    ToggleButton,
    ChildComponents
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
