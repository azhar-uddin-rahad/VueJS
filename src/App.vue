<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <HomePage/>
  <h1>Vew Event handler</h1>
  <BasicEvent></BasicEvent>
  <MakeInputForms></MakeInputForms>
  <ToggleButton></ToggleButton>
  <ChildComponents name="azhar uddin rahad" :user='user' :sendData='sendData'></ChildComponents>
  <ul >
    <li v-for="(studentData,index) in studentInfo" :key="index">
      <DynamicList :items="studentData" :getData="getData"></DynamicList>
    </li>
   
  </ul>
  <ClassBinding></ClassBinding>
  


</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import HomePage from './components/HomePage.vue'
import BasicEvent from './components/BasicEvent'
import MakeInputForms from './components/MakeInputForms'
import ToggleButton from './components/ToggleButton'
import ChildComponents from './components/ChildComponents'
import DynamicList from './components/DynamicList.vue'
import ClassBinding from './components/ClassBinding.vue'
export default {
  name: 'App',
  components: {
    HelloWorld,
    HomePage,
    BasicEvent,
    MakeInputForms,
    ToggleButton,
    ChildComponents,
    DynamicList,
    ClassBinding
    },
  data(){
    return{
      user:{name: "azhar1",email:'aur@gmail.com '},
      studentInfo:[
       { name:'biplob', email:'biplob@gmail.com'},
       { name:'shakib', email:'shikb@gmail.com'},
       { name:'jobear', email:'jobear@gmail.com'},
       { name:'mizan', email:'mizan@gmail.com'},
      ]
    }
  },
  methods: {
    sendData(){
      console.log("parent function called")
    },
    getData(name){
     alert(name)
    }
  },
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
