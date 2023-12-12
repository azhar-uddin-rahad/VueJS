<template>
<h1> home component</h1>
 <h1>Email: {{email}}</h1>
 <h1>Mobile: {{mobile}}</h1>
 <!-- <h1>Mobile: {{mobile =100}}</h1> -->
 <!-- <h1>Mobile: {{mobile ===100}}</h1> -->
  <h3>Name send on function: {{getNameFun("Azhar Form Function")}}</h3>
<!-- Method use section start -->
<h2>Full Name: {{setNameMethod()}}</h2>
<h2>CollageName:  {{getNameMethod("institute of computer science and technology")}}</h2>
<h3>under the method All data show: {{setData()}}</h3>
<h3>under the method specific data show: {{setData().email}}</h3>

</template>

<script>
export default {
  name: 'HomePage',
  data(){
    return{
      email: 'azhar@gmail.com',
      mobile: 8888,
      getNameFun:function (names) {
        return names;
        
      }
    }
  },
  methods: {
    setNameMethod(){
      return 'azhar uddin rahad';

    },
    getNameMethod(name){
      return name;
    },
    setData(){
     return{
       name: "Alif",
       email: this.email
     }
    }

  }, 
  
 
}
</script>

<style scoped>
h1{
  color: red;
}
</style>