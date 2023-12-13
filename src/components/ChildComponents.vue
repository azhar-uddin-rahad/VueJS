<template>
    <h2>Child Components </h2>
    <h2>{{ name }}</h2>

    <h1>get Data From parents components</h1>
    <p>{{ user.name }}</p>
    <button v-on:click="sendData()">Click me</button>

</template>
<script>

export default{
    name : "ChildComponents",
     props:{
          name:String,
          user: Object,
          sendData:Function
    }
}

</script>