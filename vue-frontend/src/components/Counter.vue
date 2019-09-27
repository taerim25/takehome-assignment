<template>
  <div>
    <p>I'm a Counter!</p>
    <button v-on:click="initial_count += 1">Add 1</button>
    <button v-on:click="initial_count -= 1">Subtract 1</button>
    <p>Current count: {{initial_count}}</p>
    <Instructions v-bind:complete="true"/>

  </div>
</template>

<script> 
import Instructions from "./Instructions.vue";

export default {
  
  props: {initial_count:{
    default:0
  } },
  /*
  data() {
    return {
      count: 0
    };
  }*/
  
};
</script>

<style>
</style>

