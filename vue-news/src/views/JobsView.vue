<template>
  <div>
      jobs
  </div>
</template>

<script>
import { jobsList } from '../api/index.js';
export default {
  created(){
    jobsList()
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