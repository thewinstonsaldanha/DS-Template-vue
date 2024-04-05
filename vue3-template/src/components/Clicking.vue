<template>
    

    
    <p> Count :: {{ count }}</p>

    <!-- <button @click="counter">Increment</button> -->

    <button @dblclick.once="counter">Increment</button>

</template>

<script setup>

import {ref} from 'vue';

let count= ref(0)


const counter= ()=>{
  count.value++
  console.log('clicked')
}



</script>