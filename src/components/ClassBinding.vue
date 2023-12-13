<template>
<h1>Class binding</h1>
<!-- if is using green:true this time green class is working or if i using green:false this time green class is not working  -->
<!-- <p :class="{green:true}">Color with conditions</p> -->
<p :class="{green:colorAdd}">Color with conditions</p>
<button v-on:click="colorAdd=!colorAdd">Apply style</button>

</template>
<script>
export default{
    name:"ClassBinding",
    data(){
        return{
            colorAdd:false
        }
    }
}

</script>

<style>

  .green{
    background-color: green;
    color: white;
    height: 100px;
  }
</style>