<template>
  <div>
      ask
  </div>
</template>

<script>
import { askList } from '../api/index.js';
export default {
  created(){
    askList()
    .then(function(response){
      console.log(response);
    })
    .catch(function(error){
      console.log(error);
    })
  }
}
</script>

<style>

</style>