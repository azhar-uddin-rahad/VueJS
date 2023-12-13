<template>
   <div class="showsInfo">
    <h1>{{ items.name }}</h1>
    <h1>{{ items.email }}</h1>
    <button v-on:click="getData(items.name)">More Details</button>
   </div>
</template>
<script>
export default {
    name:"DynamicList",
    props:{
        items:Object,
        getData:Function

    }

}
</script>
<style>
    .showsInfo{
        background-color: red;
        margin-bottom: 20px;
        color: #000;

    }
</style>