<template>
<h1>Show How to Work Event </h1>
<button v-on:click="test()">Counter Up</button>
 <h4>{{count}}</h4>
 <button v-on:click="openAlert()">Open Alert</button>
    <div class="TwoWayBinding">
        <h2>Tow way Bidding</h2>
        <input type="text" v-model="onChangeInputValue"/>
        <h4>{{onChangeInputValue}}</h4>
    
    </div>
    
</template>
<script>
export default {
    name: 'BasicEvent',
    data(){
         return{
         count:0,
         onChangeInputValue: 0
         }
    },
    methods:{
        test(){
            this.count=this.count+1
        },

        openAlert(){
                alert("Welcome to vew js")
        }
    }

}
</script>
<style scoped>
.TwoWayBinding{
    margin-top:100px;

}

</style>