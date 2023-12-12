<template>
  <div class="inputForms">
    <h1>Input From Data</h1>
    <input type="text" v-model="email" />
    <input type="password" v-model="password" />
    <button v-on:click="showsInputData()"> Shows Result</button>
    <br> <br>
    <label>javascript</label>
    <input type="checkbox" value="javascript" v-model="technology" id="js" />
    <br><br>
    <label>PhP</label>
    <input type="checkbox" value="php" v-model="technology" id="php"/>
    <label>Python</label>
    <input type="checkbox" value="python" v-model="technology" id="python"/>
    <h4>Shows All Technology: {{technology}}</h4>
    <p>proposition:
    <label>student</label>
    <input type="radio" value="student" name="proposition" v-model="student" id="js" />
    <br><br>
    <label>Developer</label>
    <input type="radio" value="developer" name="proposition" v-model="student" id="php"/>
  
    
    </p>
  </div>
</template>
<script>
export default {
  name: "MakeInputForms",
  data() {
    return {
      email: null,
      password: null,
      technology:[],
    };
  },
  methods:{
    showsInputData(){
       console.log(this.email,this.password)
    }
  }

};
</script>
<style scoped>
.inputForms {
  margin-top: 50px;
  margin-bottom:100px;
}
</style>
