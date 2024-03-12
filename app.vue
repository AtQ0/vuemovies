<template>
  <Header />
 <!-- <Header></Header> -->

  <main>
    <h1 @click="nameGenerator()">Hello World</h1>

  </main>



</template>

<script setup>

import './assets/css/global.css'

  //Import ref in order to enable creation of variables
  import { ref } from "vue";

  //Import used components
  import Header from "@/layouts/Header.vue"





  const name = ref("Alice")


  function nameGenerator(){

    console.log(name.value)
  }


</script>



<style scoped>




  h1{
    cursor: pointer;

  }

</style>
