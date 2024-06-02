<template>
<div class="container">
    <img class="logo" src="../assets/signup.png">
    </div>
 
  <h1> Sign Up </h1> 
  <div class="register">
    <input type="text" placeholder ="enter name"/>
    <input type="text" placeholder ="enter Email"/>
    <input type="text" placeholder ="enter password"/>
    <button v-on:click="signUp"> register </button>
    

    </div>
</template>

<script>
export default {
 name : 'SignUp',
 methods:{
    signUp(){
       this.$router.push({name:'HomePage'})
    }
 }
}
</script>

<style>
.container {
      display: flex;
      justify-content: center;
      align-items: center;
       /* 100% de la hauteur de la fenêtre */
    }
.logo {
    width: 100px;
}
.register input{
   width : 300px;
   height: 40px;
   padding-left :20px;
   display:block;
   margin-bottom:30px;
   margin-right:auto;
   margin-left:auto;
   border : 1px solid skyblue;

}
.register button{
    width: 320px;
    height:40px;
    border: 1px solid skyblue;
    background: rgb(5, 63, 86);
    color: #fff;
    cursor:pointer;
}

</style>