<template>
<h1>iF else conation </h1>
<p>if shows value is true is time run if condition running or if shows value is false this time else conditions is running</p>
<div>
<h1 v-if="shows">if conditions running</h1>

<h1 v-else>else conditions running</h1>


<button @click="toggle =!toggle">Toggle Button</button>
    <h1 v-if="toggle">Ami Asi</h1>
</div>




</template>
<script>
export default{
    name: "ToggleButton",
    data(){
        return{
            shows:false,
            toggle:false
        }
    }
}


</script>