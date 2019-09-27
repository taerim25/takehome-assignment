<template>
  <!-- PART 4: Add your code here -->
  <!-- it doesn't seem to import Counter correctly, thus not showing the counter as intended-->
  <div>
    {{name}}
    <Counter v-bind:initial_count = "episodes_seen"></Counter>
  </div>
</template>

<script>
// PART 4: Add your code here
import Counter from "./Counter.vue";

export default {
  props:['id','name','episodes_seen']
  
};
</script>

<style>
</style>
