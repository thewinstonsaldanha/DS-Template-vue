<template>
    <h1> This is from Counter</h1>

     <!-- On the screen -->
    <p>{{ state.count }}</p> 

     <!-- On the console -->
    <p>{{ state.increment }}</p>

    
    <!-- Using Counter -->
    <p>{{ counter }}</p>

    <button @click="increment()">Click Here</button>
</template>

<script setup>
//import reactivity
import {reactive, ref} from 'vue';
const state= reactive({count: 0});
const counter= ref(10)

const increment=()=>{
    console.log("Incremented");
    state.count++;
    counter.value++;
}

</script>

<style >

</style>